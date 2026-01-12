<!-- ======= PULSE MONUMENT PARENT (HTML-низ) ======= -->
<script>
(function () {
  console.log("🧱 PULSE Monument Parent initialized");

  const APP_ID = 16777213;
  const STORAGE_KEY_PROGRESS = "pulseMonumentGame";

  const CONFIG = {
    TOPIC_ID: 21,
    LIMIT_POSTS: 200,     // максимум API = 200
    LOG_LIMIT: 60
  };

  const STAGES_BASE = {
    "Основание":     { need: 600, have: 0 },
    "Фракции":       { need: 300, have: 0 },
    "Логотип PULSE": { need: 300, have: 0 },
    "Подсветка":     { need: 350, have: 0 },
    "Символ":        { need: 450, have: 0 }
  };

  const ITEM_TO_STAGE = {
    "Кирпич":"Основание","Булыжник":"Основание","Плита из бетона":"Основание","Обломок колонны":"Основание",
    "Осколок эмблемы":"Фракции","Фрагмент знамени":"Фракции","Жетон фракции":"Фракции",
    "Металлическая пластина":"Логотип PULSE","Ржавая балка":"Логотип PULSE","Арматура":"Логотип PULSE","Титановый лист":"Логотип PULSE",
    "Светодиод":"Подсветка","Блок питания":"Подсветка","Кабель подсветки":"Подсветка",
    "Цемент":"Символ","Гипсовый раствор":"Символ","Каменная крошка":"Символ"
  };

  // --- утилиты ---
  function deepClone(x){ return JSON.parse(JSON.stringify(x)); }

  function decodeHtmlEntities(str) {
    if (!str) return "";
    // на форумах часто прилетает &lt;span ...&gt;
    const ta = document.createElement("textarea");
    ta.innerHTML = str;
    return ta.value;
  }

  function safeText(x){ return (x == null) ? "" : String(x); }

  function clamp(n,a,b){ return Math.max(a, Math.min(b, n)); }

  // --- API helpers ---
  function apiGet(method, params) {
    return new Promise((resolve, reject) => {
      $.get("/api.php", { token: ForumAPITicket, method, app_id: APP_ID, ...params }, (resp) => {
        if (!resp || resp.error || resp.errors) reject(resp);
        else resolve(resp);
      }, "json").fail((xhr) => reject(xhr));
    });
  }

  function storageSet(key, valueObj) {
    return new Promise((resolve) => {
      $.post("/api.php",
        { token: ForumAPITicket, method: "storage.set", app_id: APP_ID, key, value: JSON.stringify(valueObj) },
        (response) => resolve(response || {}),
        "json"
      ).fail(() => resolve({ error: true, reason: "network_fail" }));
    });
  }

  function storageGetRaw(key) {
    return new Promise((resolve) => {
      $.get("/api.php",
        { token: ForumAPITicket, method: "storage.get", app_id: APP_ID, key },
        (response) => resolve(response?.response?.storage?.data?.[key] || null),
        "json"
      ).fail(() => resolve(null));
    });
  }

  // --- парсер pulse-donate через DOM (без регулярок) ---
  function extractDonatesFromMessage(messageHtml) {
    const rows = [];
    if (!messageHtml) return rows;

    const decoded = decodeHtmlEntities(messageHtml);

    const box = document.createElement("div");
    // иногда там бывает мусор, но нам важны только span.pulse-donate
    box.innerHTML = decoded;

    const spans = box.querySelectorAll("span.pulse-donate");
    spans.forEach((sp) => {
      const ds = sp.dataset || {};
      const item = safeText(ds.item).trim();
      const qty = parseInt(ds.qty || "1", 10) || 1;
      const user = safeText(ds.user || "—").trim();
      const time = safeText(ds.time || "").trim();
      const url  = safeText(ds.url || "").trim();
      const key  = safeText(ds.key || "").trim();

      const stage = ITEM_TO_STAGE[item];
      rows.push({
        key: key || `${user}|${item}|${time}|${url}|${Math.random().toString(16).slice(2)}`,
        user, item, qty, time, url,
        stage: stage || null
      });
    });

    return rows;
  }

  function compute(rows) {
    const stages = deepClone(STAGES_BASE);

    const perUser = {};
    const unknown = {};     // что не сопоставилось
    const seenKeys = new Set(); // защита от дублей (если случайно один и тот же span дважды в HTML)

    let counted = 0;
    let skippedDup = 0;

    rows.forEach(r => {
      if (seenKeys.has(r.key)) { skippedDup++; return; }
      seenKeys.add(r.key);

      if (!r.item) {
        unknown["(пусто)"] = (unknown["(пусто)"] || 0) + 1;
        return;
      }

      if (!r.stage) {
        unknown[r.item] = (unknown[r.item] || 0) + 1;
        return;
      }

      if (!stages[r.stage]) return;

      stages[r.stage].have += r.qty;
      counted += r.qty;

      if (!perUser[r.user]) perUser[r.user] = { total: 0, stages: {} };
      perUser[r.user].total += r.qty;
      perUser[r.user].stages[r.stage] = (perUser[r.user].stages[r.stage] || 0) + r.qty;
    });

    const stageList = Object.entries(stages);
    const totalNeed = stageList.reduce((s, [, v]) => s + (v.need||0), 0);
    const totalHave = stageList.reduce((s, [, v]) => s + Math.min((v.have||0), (v.need||0)), 0);
    const totalPct  = totalNeed ? Math.floor((totalHave / totalNeed) * 100) : 0;

    const lastLogs = rows
      .filter(r => r.item && r.stage) // только валидные
      .slice(-CONFIG.LOG_LIMIT)
      .reverse()
      .map(r => ({ user:r.user, item:r.item, qty:r.qty, stage:r.stage, time:r.time, url:r.url }));

    return {
      stages,
      total: { need: totalNeed, have: totalHave, pct: clamp(totalPct, 0, 100) },
      lastLogs,
      perUser,
      unknown,
      debug: { foundSpans: rows.length, counted, skippedDup }
    };
  }

  let CACHE = { ts: 0, payload: null };

  async function recalc() {
    if (typeof ForumAPITicket === "undefined" || !ForumAPITicket) {
      return { ok: false, error: "ForumAPITicket missing (parent должен быть в HTML-низ и работать на страницах темы)" };
    }

    const resp = await apiGet("post.get", {
      topic_id: CONFIG.TOPIC_ID,
      fields: "id,username,message",
      limit: CONFIG.LIMIT_POSTS
    });

    const list = resp?.response || [];
    if (!Array.isArray(list) || !list.length) {
      return { ok: false, error: "post.get returned empty", raw: resp };
    }

    // иногда первая “шапка” тоже пост — норм, мы считаем только pulse-donate
    let all = [];
    list.forEach(p => { all = all.concat(extractDonatesFromMessage(p.message)); });

    const payload = {
      updatedAt: new Date().toISOString(),
      topicId: CONFIG.TOPIC_ID,
      scannedPosts: list.length,
      data: compute(all)
    };

    const save = await storageSet(STORAGE_KEY_PROGRESS, payload);
    if (save?.error || save?.errors) {
      return { ok: false, error: "storage.set failed", save };
    }

    CACHE = { ts: Date.now(), payload };
    return { ok: true, payload };
  }

  async function getStatus() {
    if (CACHE.payload && (Date.now() - CACHE.ts) < 15000) {
      return { ok: true, payload: CACHE.payload, cached: true };
    }

    const raw = await storageGetRaw(STORAGE_KEY_PROGRESS);
    if (!raw) return { ok: true, payload: null };

    try {
      const payload = JSON.parse(raw);
      CACHE = { ts: Date.now(), payload };
      return { ok: true, payload };
    } catch (e) {
      return { ok: false, error: "bad json in storage" };
    }
  }

  // --- PUBLIC OBJECT (как у MonsterBattleAdmin) ---
  window.PulseMonumentParent = {
    recalc,
    getStatus,
    dump: async () => (await getStatus())
  };

  // --- postMessage bridge ---
  window.addEventListener("message", async function (event) {
    const data = event.data;
    if (!data?._pulseMonument || data.type !== "request") return;

    let result;
    try {
      if (data.action === "getStatus") result = await getStatus();
      else if (data.action === "recalc") result = await recalc();
      else result = { ok: false, error: "Unknown action: " + data.action };
    } catch (e) {
      // чтобы не было [object Object]
      try { result = { ok:false, error: JSON.stringify(e) }; }
      catch { result = { ok:false, error: String(e) }; }
    }

    event.source?.postMessage({
      _pulseMonument: true,
      type: "response",
      requestId: data.requestId,
      result
    }, event.origin);
  });

})();
</script>
<!-- ======= /PULSE MONUMENT PARENT ======= -->
