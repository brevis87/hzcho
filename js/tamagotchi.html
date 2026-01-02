<div class="tama-title" style="display:none;">Тамагочи-Зомби</div>



<style>

#wrap { 
    background: url('https://upforme.ru/uploads/001c/84/76/2/180199.png') no-repeat center;
    background-size: 100% 100%;
    height: 100%; 
    width: 100%;
position: relative;
    overflow: hidden; 
    color: #000; 
    padding: 50px; /* Чуть уменьшил padding, чтобы влезло больше контента */
    font-family: 'Arial', sans-serif; 
    display: grid; 
    grid-template-columns: 160px 1fr 300px; /* Немного расширил левую под ТОП */
    gap: 50px; /* Уменьшил зазор между колонками (было 70) */
    box-sizing: border-box; 
}

.paper-block { background: #e9e5d3; padding: 15px; position: relative; display: flex; flex-direction: column; }

.block-title { font-size: 18px; font-weight: bold; text-transform: uppercase; border-bottom: 2px solid #333; margin-bottom: 10px; padding-bottom: 5px; }

/* Указываем левой колонке занять всю доступную высоту */
.left-col { 
    display: flex; 
    flex-direction: column; 
    gap: 20px; 
    height: 100%; 
}

/* Настройки ТОПа: разрешаем ему расти и добавляем прокрутку */
#rating { 
    font-size: 15px; 
    line-height: 1.8; 
    font-weight: bold; 
    overflow-y: auto; /* Появится скролл, если игроков много */
    flex-grow: 1;     /* Заставит блок растянуться до счетчиков */
    padding-right: 5px; /* Отступ, чтобы скролл не налезал на текст */
}

/* Ограничиваем высоту родительского блока ТОПа, чтобы он не выталкивал счетчики за экран */
.left-col .paper-block:first-child {
    flex-grow: 1;
    max-height: 500px; /* Настройте это число под ваш экран, чтобы ТОП не был слишком длинным */
    display: flex;
    flex-direction: column;
}

.rating-item { display: flex; justify-content: space-between; border-bottom: 1px dashed #999; }

.counters-area { 
    margin-top: -8px; /* Прижмет блок к низу левой колонки */
    padding: 10px;    /* Уменьшили внутренние отступы, чтобы сжать блок */
}

.counter-row { 
    display: flex; 
    align-items: center; 
    gap: 5px; 
    margin-bottom: 8px; /* Уменьшили расстояние между строками (было 15) */
    background: rgba(0,0,0,0.03); /* Легкая подложка как на картинке */
    padding: 5px;
}

/* Контейнер для текста и цифр внутри строки */
.counter-info-container {
    display: flex;
    justify-content: space-between; /* РАССТАЛКИВАЕТ текст влево, а число вправо */
    align-items: flex-start;
    width: 100%; /* Занимает всё оставшееся место справа от иконки */
}

.counter-row img { width: 35px; height: 35px; }

/* Стили заголовков (Доступно действий / Бонусных) */
.counter-label { 
    font-size: 10px; 
    font-weight: 900; 
    text-transform: uppercase;
    line-height: 1.2;
    color: #222;
}

/* Стили больших цифр справа */
.counter-val { 
    font-size: 28px; 
    font-weight: 900; 
    color: #008b8b; 
    line-height: 1;
}

/* Дополнительный текст под заголовком */
.reset-timer, .counter-subtext {
    font-size: 11px;
    font-weight: bold;
    margin-top: 5px;
}

.reset-timer { font-size: 11px; color: #b22222; font-weight: bold; margin-top: 4px; }

.center-col { display: flex; flex-direction: column; align-items: center; }

.time-bubble { background: #e9e5d3; padding: 10px 20px; font-size: 18px; font-weight: bold; margin-bottom: 20px; }

.zombie-display { width: 300px; height: 350px; position: relative; display: flex; justify-content: center; align-items: center; margin-bottom: 20px; overflow: visible; /* Чтобы части слишком большой гифки не вылезали за края */ }

.zombie-display img { 
width: 350px;          /* Задайте ту ширину, которая вам кажется идеальной */
    height: 350px;         /* Задайте ту же высоту, чтобы область была квадратной */
    object-fit: contain;   /* ВАЖНО: это впишет гифку в квадрат 250x250 без искажений и обрезки */
    position: absolute;    /* Чтобы они накладывались друг на друга в одной точке */
    transition: 0.3s;      /* Плавность (по желанию) */
bottom: -80px;
}

.stats-wrap { width: 100%; max-width: 450px; margin-top: 80px; }

.stat-row { margin-bottom: 10px; }

.stat-head { display: flex; justify-content: space-between; font-size: 11px; font-weight: bold; color: #fff; text-transform: uppercase; margin-bottom: 3px; }

.bar { height: 14px; background: #222; border: 1px solid #444; }

.fill { height: 100%; transition: width 0.5s ease-in-out; }

.right-col { display: flex; flex-direction: column; gap: 20px; }

.action-btn { background: none; border: 1px solid transparent; display: flex; align-items: center; padding: 6px; cursor: pointer; text-align: left; width: 100%; transition: 0.2s; }

.action-btn:hover:not(:disabled) { background: rgba(0,0,0,0.05); border-color: #999; }

.action-btn:disabled { opacity: 0.5; filter: grayscale(1); cursor: not-allowed; }

.action-btn img { width: 42px; height: 42px; margin-right: 12px; }

.act-name { display: block; font-size: 17px; font-weight: bold; text-transform: uppercase; }

.act-desc { display: block; font-size: 10px; color: #555; }

#logs { height: 150px; overflow-y: auto; font-size: 11px; font-family: monospace; background: rgba(255,255,255,0.2); padding: 8px; border: 1px solid #ccc; }

.death-message { color: #f44 !important; font-weight: bold; }

.admin-message { color: #007bff !important; font-weight: bold; }

.emotion-indicator { position: absolute; top: 0; left: 50%; transform: translateX(-50%); background: rgba(0,0,0,0.8); color: #fff; padding: 5px 15px; border-radius: 20px; font-size: 12px; opacity: 0; transition: 0.3s; z-index: 10; }

.emotion-indicator.show { opacity: 1; top: -20px; }

.loading-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: #111; z-index: 9999; display: flex; align-items: center; justify-content: center; color: #fff; }

/* Кнопка в углу */
.info-btn-wrapper {
    position: absolute;
    top: 10px;
    right: 10px;
    z-index: 100;
line-height: 0; /* Убирает лишние отступы снизу у картинки */
}

.info-icon {
    width: 45px;
    height: 45px;
    cursor: pointer;
    transition: transform 0.2s, filter 0.2s;
    filter: drop-shadow(2px 2px 2px rgba(0,0,0,0.5));
}

.info-icon:hover {
    transform: scale(1.1);
}

/* Модальное окно */
.info-modal {
    display: none; /* Скрыто по умолчанию */
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.7);
    z-index: 2000;
    justify-content: center;
    align-items: center;
}

.info-content {
    width: 350px;
    max-height: 80vh;
    overflow-y: auto;
    animation: fadeIn 0.3s ease;
}

.info-text {
    font-size: 13px;
    line-height: 1.4;
    color: #333;
}

.info-text ul {
    padding-left: 20px;
    margin: 10px 0;
}

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(-20px); }
    to { opacity: 1; transform: translateY(0); }
}

</style>



<div id="wrap">

<div class="info-btn-wrapper">
    <img src="https://upforme.ru/uploads/001c/84/76/2/414706.png" class="info-icon" onclick="toggleInfoModal()" title="Информация об игре">
</div>

<div id="infoModal" class="info-modal">
    <div class="info-content paper-block">
        <div class="block-title">📖 Инструкция</div>
        <div class="info-text">
            <p><b>Цель игры:</b> Поддерживать жизнь зомби как можно дольше.</p>
            <ul>
                <li><b>Сытость:</b> Падает быстрее всего. Кормите вовремя.</li>
                <li><b>Инфекция:</b> Если она выше 85%, здоровье начнет быстро уходить.</li>
                <li><b>Настроение:</b> Если упадет ниже 15%, зомби начнет терять здоровье от тоски.</li>
                <li><b>Активность:</b> При уровне ниже 10% наносится дополнительный урон.</li>
                <li><b>Регенерация:</b> Если настроение выше 90% и инфекция низкая, здоровье зомби постепенно восстанавливается само.</li>
                <li><b>Смерть:</b> Если здоровье упадет до 0, действия блокируются до воскрешения администратором.</li>

            </ul>
            <p><i>Ночью (00:00 - 08:00) показатели падают на 10% медленнее.</i></p>
        </div>
        <button class="action-btn" onclick="toggleInfoModal()" style="margin-top:15px; justify-content:center;"><b>ЗАКРЫТЬ</b></button>
    </div>
</div>

    <div id="loadingOverlay" class="loading-overlay">ЗАГРУЗКА...</div>

    <div class="left-col">

        <div class="paper-block">

            <div class="block-title">🏆 ТОП ИГРОКОВ</div>

            <div id="rating"></div>

        </div>

<div class="paper-block counters-area">

    <div class="counter-row">
        <img src="https://upforme.ru/uploads/001c/84/76/2/177104.png">
        <div class="counter-info-container">
            <div>
                <div class="counter-label">ДОСТУПНО<br>ДЕЙСТВИЙ</div>
                <div id="actionsTimer" class="reset-timer" style="color: #8eb93b;">обновление через 00:00:00</div>
            </div>
            <div class="counter-val" id="actionsCounter">9/9</div>
        </div>
    </div>

    <div class="counter-row">
        <img src="https://upforme.ru/uploads/001c/84/76/2/662919.png">
        <div class="counter-info-container">
            <div>
                <div class="counter-label" style="color: #b22222;">БОНУСНЫХ<br>ДЕЙСТВИЙ</div>
                <div class="counter-subtext" style="color: #d112bb;">*покупается за игровую валюту</div>
            </div>
            <div class="counter-val" id="bonusActions" style="color: #b22222;">0</div>
        </div>
    </div>

</div>

    </div>

    <div class="center-col">

        <div class="time-bubble">Зомби прожил: <span id="aliveInfo" style="color:#8eb93b">0 д., 0 ч.</span></div>

        <div class="zombie-display">

            <div id="emotionIndicator" class="emotion-indicator"></div>

            <img id="zombieImage" src="https://upforme.ru/uploads/001c/84/76/2/443090.gif">

            <img id="happyGif" src="https://upforme.ru/uploads/001c/84/76/2/925156.gif" style="display:none; position:absolute;">

            <img id="angryGif" src="https://upforme.ru/uploads/001c/84/76/2/171339.gif" style="display:none; position:absolute;">

            <img id="sadImage" src="https://upforme.ru/uploads/001c/84/76/2/581889.gif" style="display:none; position:absolute;">

            <img id="deadZombieImage" src="https://upforme.ru/uploads/001c/84/76/2/313667.gif" style="display:none; position:absolute;">

        </div>

        <div class="stats-wrap">

            <div class="stat-row"><div class="stat-head"><span>Здоровье</span> <span id="hpValue">0</span>/100</div><div class="bar"><div id="hp" class="fill" style="background:red;"></div></div></div>

            <div class="stat-row"><div class="stat-head"><span>Сытость</span> <span id="hungerValue">0</span>/100</div><div class="bar"><div id="hunger" class="fill" style="background:orange;"></div></div></div>

            <div class="stat-row"><div class="stat-head"><span>Настроение</span> <span id="moodValue">0</span>/100</div><div class="bar"><div id="mood" class="fill" style="background:deepskyblue;"></div></div></div>

            <div class="stat-row"><div class="stat-head"><span>Активность</span> <span id="activityValue">0</span>/100</div><div class="bar"><div id="activity" class="fill" style="background:limegreen;"></div></div></div>

            <div class="stat-row"><div class="stat-head"><span>Инфекция</span> <span id="infectionValue">0</span>/100</div><div class="bar"><div id="infection" class="fill" style="background:purple;"></div></div></div>

        </div>

    </div>

    <div class="right-col">

        <div class="paper-block">

            <div class="block-title">ДЕЙСТВИЯ</div>

            <button class="action-btn" onclick="doAction('feed')"><img src="https://upforme.ru/uploads/001c/84/76/2/476415.png"><span><span class="act-name">Кормить</span><span class="act-desc">+30 сытость, -5 активность</span></span></button>

            <button class="action-btn" onclick="doAction('play')"><img src="https://upforme.ru/uploads/001c/84/76/2/671196.png"><span><span class="act-name">Развлечь</span><span class="act-desc">+25 настроение</span></span></button>

            <button class="action-btn" onclick="doAction('heal')"><img src="https://upforme.ru/uploads/001c/84/76/2/818211.png"><span><span class="act-name">Лечить</span><span class="act-desc">+15 здоровье, -40 инфекция</span></span></button>

            <button class="action-btn" onclick="doAction('energize')"><img src="https://upforme.ru/uploads/001c/84/76/2/998081.png"><span><span class="act-name">Взбодрить</span><span class="act-desc">+35 активность, -10 настроение</span></span></button>

            <button class="action-btn" onclick="doAction('sabotage')"><img src="https://upforme.ru/uploads/001c/84/76/2/493297.png"><span><span class="act-name">Саботаж</span><span class="act-desc">+15 инф.</span></span></button>

        </div>

        <div class="paper-block" style="margin-top: 90px;"><div class="block-title">📝 ЖУРНАЛ</div><div id="logs"></div></div>

    </div>

</div>



<script>
const KEY = "GLOBAL_ZOMBIE_TAMA";
const APP = 16777213;
const USER = window.UserLogin || "Игрок";
const MAX_ACTIONS = 9;
let state = null;
let lastRequestTime = 0;
let isAnimating = false;

// Вспомогательные функции времени
function getMoscowNow() { return new Date(new Date().getTime() + (new Date().getTimezoneOffset() * 60000) + (3 * 3600000)); }
function getMoscowDateStr() { return getMoscowNow().toISOString().split('T')[0]; }
function getFullLogDate() { const n = new Date(); return `${n.getDate().toString().padStart(2,'0')}.${(n.getMonth()+1).toString().padStart(2,'0')} ${n.getHours().toString().padStart(2,'0')}:${n.getMinutes().toString().padStart(2,'0')}`; }

class API {
    static async get() {
        if (Date.now() - lastRequestTime < 2000) return null;
        lastRequestTime = Date.now();
        try {
            const resp = await fetch(`/api.php?token=${window.ForumAPITicket || ''}&method=storage.get&app_id=${APP}&key=${KEY}`);
            const json = await resp.json();
            const raw = json?.response?.storage?.data?.[KEY];
            if(!raw) return null;
            const parsed = JSON.parse(raw);
            return parsed.data || parsed;
        } catch (e) { return null; }
    }
    static async set(data) {
        lastRequestTime = Date.now();
        const fd = new FormData();
        fd.append('token', window.ForumAPITicket || '');
        fd.append('method', 'storage.set');
        fd.append('app_id', APP);
        fd.append('key', KEY);
        fd.append('value', JSON.stringify({ data }));
        await fetch('/api.php', { method: 'POST', body: fd });
    }
}

// ГЛАВНЫЙ ЦИКЛ ИЗМЕНЕНИЙ (с учетом оффлайна)
let isSyncing = false; // Добавьте в начало скрипта к остальным let

async function gameTick() {
    if (isSyncing) return; // Если запрос уже идет, не начинаем новый
    isSyncing = true;

    const remote = await API.get();
    // Обновляем состояние ТОЛЬКО если мы сейчас не заняты анимацией
    if (remote && !isAnimating) state = remote;
    
    if (!state || state.isDead) {
        isSyncing = false;
        return;
    }

    const now = Date.now();
    const elapsedMs = now - (state.lastUpdate || now);
    const intervals = Math.max(0, Math.floor(elapsedMs / 15000)); 

    for(let i = 0; i < intervals; i++) {
        const checkTime = new Date((state.lastUpdate || now) + (i * 15000));
        const hour = (checkTime.getUTCHours() + 3) % 24;
        const isNight = (hour >= 0 && hour < 8);
        const factor = isNight ? 0.2 : 1.0; 

        state.hunger = Math.max(0, state.hunger - (0.2 * factor));
        state.mood = Math.max(0, state.mood - (0.15 * factor));
        state.activity = Math.max(0, state.activity - (0.15 * factor));
        state.infection = Math.min(100, state.infection + (0.15 * factor));
        
        let hpChange = 0;
        // ШТРАФЫ
        if (state.hunger < 15) hpChange -= 0.8;  
        if (state.infection > 70) hpChange -= 0.6;
        if (state.infection > 90) hpChange -= 1.2;
        if (state.mood < 15) hpChange -= 0.5;
        if (state.activity < 10) hpChange -= 0.3;

        // БОНУСЫ
        if (state.mood > 90 && state.infection < 30) {
            hpChange += 0.4; 
        }

        if (hpChange < 0) {
            state.hp = Math.max(0, state.hp + (hpChange * factor));
        } else if (hpChange > 0) {
            state.hp = Math.min(100, state.hp + hpChange);
        }

        if (state.hp <= 0) {
            state.isDead = true;
            state.hp = 0;
            const exactDeathTime = (state.lastUpdate || now) + (i * 15000);
            state.timeOfDeath = exactDeathTime;
            const d = new Date(exactDeathTime);
            const deathDateStr = `${d.getDate().toString().padStart(2,'0')}.${(d.getMonth()+1).toString().padStart(2,'0')} ${d.getHours().toString().padStart(2,'0')}:${d.getMinutes().toString().padStart(2,'0')}`;

            state.logs.unshift({ 
                text: `💀 ${deathDateStr} - ЗОМБИ ПОГИБ! (в ваше отсутствие).`, 
                cssClass: 'death-message' 
            });
            break; 
        }
    } // Конец цикла for

    state.lastUpdate = now;
    render();
    await API.set(state);
isSyncing = false;
}

// ФУНКЦИЯ ВОСКРЕШЕНИЯ (вызывается вашим админ-скриптом)
async function resurrect() {
    const remote = await API.get();
    if (remote) state = remote;

    state.isDead = false;
    state.hp = 80;      
    state.hunger = 70;
    state.mood = 70;
    state.activity = 70;
    state.infection = 5;
    state.createdAt = Date.now(); // Сброс времени жизни (новый цикл)
    state.actions = {}; // ОБНУЛЕНИЕ ДЕЙСТВИЙ: теперь у всех снова 9/9
    state.timeOfDeath = null;
    
    state.logs.unshift({ 
        text: `⚡ ${getFullLogDate()} - ВОСКРЕШЕНИЕ: Зомби снова в строю! Лимиты действий восстановлены.`, 
        cssClass: 'admin-message' 
    });

state.lastUpdate = Date.now();
    render();
    await API.set(state);
    isSyncing = false; // Открываем доступ для следующего цикла
}

function render() {
    if (!state) return;
    
    const now = getMoscowNow();
    
    // ТАЙМЕР СБРОСА
    if (state.isDead) {
        document.getElementById('actionsTimer').textContent = `До сброса: 00:00:00`;
    } else {
        const midnight = new Date(now); midnight.setHours(24, 0, 0, 0);
        const diffT = midnight - now;
        document.getElementById('actionsTimer').textContent = `До сброса: ${Math.floor(diffT/3600000).toString().padStart(2,'0')}:${Math.floor((diffT%3600000)/60000).toString().padStart(2,'0')}:${Math.floor((diffT%60000)/1000).toString().padStart(2,'0')}`;
    }
    
    ['hp', 'hunger', 'mood', 'activity', 'infection'].forEach(s => {
        const val = Math.round(state[s]);
        document.getElementById(`${s}Value`).textContent = val;
        document.getElementById(s).style.width = val + '%';
    });

    // ВРЕМЯ ЖИЗНИ (замораживается при смерти)
    const endTime = state.isDead ? (state.timeOfDeath || state.lastUpdate) : Date.now();
    const deathTime = endTime - state.createdAt;
    const days = Math.floor(deathTime / 86400000);
    const hours = Math.floor((deathTime % 86400000) / 3600000);
    document.getElementById('aliveInfo').textContent = `${days} д., ${hours} ч.`;
    
    document.getElementById('rating').innerHTML = Object.entries(state.rating || {}).sort((a,b) => b[1]-a[1]).slice(0, 5).map(([n, s], i) => `<div class="rating-item"><span>${i+1}. ${n}</span><span style="color:#008080">${s}</span></div>`).join('');
    document.getElementById('logs').innerHTML = state.logs.map(l => `<div class="${l.cssClass}">${l.text}</div>`).join('');

    const today = getMoscowDateStr();
    const used = state.actions[USER]?.[today] || 0;
    const bonus = parseInt(state.bonuses?.[USER] || 0); 
    const leftActions = state.isDead ? 0 : Math.max(0, MAX_ACTIONS - used);
    
    // Если мертв, показываем 0, если жив - остаток
    document.getElementById('actionsCounter').textContent = state.isDead ? `0/9` : `${leftActions}/9`;
    document.getElementById('bonusActions').textContent = ` ${bonus}`;
    
    // БЛОКИРОВКА КНОПОК
    document.querySelectorAll('.action-btn').forEach(b => {
        b.disabled = state.isDead || (leftActions <= 0 && bonus <= 0);
    });

    if (!isAnimating) {
        ['zombieImage', 'happyGif', 'angryGif', 'sadImage', 'deadZombieImage'].forEach(id => document.getElementById(id).style.display = 'none');
        if (state.isDead) {
            document.getElementById('deadZombieImage').style.display = 'block';
        } else if (state.hp < 25) {
            document.getElementById('sadImage').style.display = 'block';
        } else {
            document.getElementById('zombieImage').style.display = 'block';
        }
    }
}

async function doAction(type) {
    if (state.isDead || isAnimating || isSyncing) return;
    isSyncing = true; 

    // 1. ПЕРЕД действием всегда берем актуальные данные с сервера
    const remote = await API.get();
    if (remote) state = remote;
    if (state.isDead) { render(); isSyncing = false; return; }

    const today = getMoscowDateStr();
    if (!state.actions[USER]) state.actions[USER] = {};
    if (!state.bonuses) state.bonuses = {};
    
    let usedToday = state.actions[USER][today] || 0;
    let bonus = parseInt(state.bonuses[USER] || 0);

    if (usedToday < MAX_ACTIONS) {
        usedToday++;
        state.actions[USER][today] = usedToday;
    } else if (bonus > 0) {
        bonus--;
        state.bonuses[USER] = bonus;
    } else { isSyncing = false; return; }

    // Применяем изменения...
    state.rating[USER] = (state.rating[USER] || 0) + 1;
    const up = (s, v) => state[s] = Math.min(100, state[s] + v);
    const down = (s, v) => state[s] = Math.max(0, state[s] - v);

    let actName = "";
    if (type === 'feed') { up('hunger', 30); down('activity', 5); actName = "покормил Зомби"; showEmotion('happy'); }
    if (type === 'play') { up('mood', 25); up('infection', 2); down('activity', 5); actName = "развлек Зомби"; showEmotion('happy'); }
    if (type === 'heal') { up('hp', 15); down('infection', 40); actName = "полечил Зомби"; showEmotion('happy'); }
    if (type === 'energize') { up('activity', 35); down('mood', 10); actName = "взбодрил Зомби"; showEmotion('happy'); }
    if (type === 'sabotage') { up('infection', 15); down('mood', 10); actName = "совершил саботаж"; showEmotion('angry'); }

    state.logs.unshift({ 
        text: `${getFullLogDate()} - ${USER} ${actName}.`, 
        cssClass: type === 'sabotage' ? 'death-message' : '' 
    });
    
    // Ограничиваем лог, чтобы он не раздувал файл (из-за этого тоже бывают лаги)
    state.logs = state.logs.slice(0, 40);
    state.lastUpdate = Date.now();

    render();
    await API.set(state); // Сохраняем обновленную версию
    isSyncing = false; 
}

function showEmotion(type) {
    if (state.isDead) return;
    isAnimating = true;
    const indicator = document.getElementById('emotionIndicator');
    ['zombieImage', 'happyGif', 'angryGif', 'sadImage', 'deadZombieImage'].forEach(id => document.getElementById(id).style.display = 'none');
    
    if (type === 'happy') { 
        document.getElementById('happyGif').style.display = 'block'; 
        indicator.textContent = 'Зомби доволен!'; 
    } else if (type === 'angry') { 
        document.getElementById('angryGif').style.display = 'block'; 
        indicator.textContent = 'Зомби в ярости!'; 
    }
    
    indicator.classList.add('show');
    setTimeout(() => { 
        indicator.classList.remove('show'); 
        isAnimating = false; 
        render(); 
    }, 3000);
}

async function autoSync() {
    const remote = await API.get();
    if (remote && JSON.stringify(remote) !== JSON.stringify(state)) { 
        state = remote; 
        render(); 
    }
}

async function init() {
    state = await API.get();
    if (!state) { 
        state = { 
            hp: 75, hunger: 65, mood: 60, activity: 55, infection: 35, 
            createdAt: Date.now(), lastUpdate: Date.now(), logs: [], 
            rating: {}, actions: {}, bonuses: {}, isDead: false 
        };
        await API.set(state);
    }
    document.getElementById('loadingOverlay').style.display = 'none';
    render();
    
    // ОСТАВЛЯЕМ ТОЛЬКО ЭТО:
    setInterval(render, 1000);    // Для плавности таймеров
    setInterval(gameTick, 20000); // Раз в 20 секунд: считаем износ и синхронимся с сервером
}
init();

function toggleInfoModal() {
    const modal = document.getElementById('infoModal');
    if (modal.style.display === 'flex') {
        modal.style.display = 'none';
    } else {
        modal.style.display = 'flex';
    }
}

// Закрытие окна при клике вне его контента
window.onclick = function(event) {
    const modal = document.getElementById('infoModal');
    if (event.target == modal) {
        modal.style.display = "none";
    }
}
</script>
