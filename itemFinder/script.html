<!--------------рандом выпадение предметов-------------->
<script>

const ril_TMPL = {
    // Карточка в теме (HTML!!!)
    IMAGE_IN_TOPIC: `
        <div class="random-image-container" style="position: absolute; z-index:1;">
            <label for="random-image-checkbox-{{id}}" class="random-image-label" style="cursor: pointer; display: inline-block;">
                <img src="https://upforme.ru/uploads/001c/84/76/2/774759.png" 
                     alt="{{name}}"
                     title="ингредиент"
                     class="glow-image" 
                     style="max-height: 100px; width: auto; display: inline-block;"
                     onload="this.parentNode.parentNode.style.left=Math.random()*600+'px'">
            </label>
        </div>
    `,
            
            // Инвентарь (BB)
    	INVENTORY: `
[b]Инвентарь пользователя[/b]
[html]
<style>
	.usr_inv {display: grid;gap: 10px;margin-top: 10px;grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));}
	.inv_item {background: ;border: 1px solid #ddd;border-radius: 4px;padding: 10px;text-align: center;}
	.item-image {width: 64px;height: 64px;object-fit: cover;border-radius: 4px;}
	.item-description {display: none;}
	#detailed-view-{{uniq}}:checked ~ .usr_inv {grid-template-columns: 1fr;}
	#detailed-view-{{uniq}}:checked ~ .usr_inv .inv_item {display: flex;align-items: center;text-align: left;gap: 15px;padding: 15px;}
	#detailed-view-{{uniq}}:checked ~ .usr_inv .item-image {width: 50px;height: 50px;flex-shrink: 0;}
	#detailed-view-{{uniq}}:checked ~ .usr_inv .item-description {display: block;flex: 1;}
</style>

<div>

	<div class="usr_inv">
    {{items}}
	</div>
</div>
[/html]
[b]Последнее обновление:[/b] {{currentTime}}
    	`,
            
// Карточка в инвентаре (HTML)
IMAGE_IN_INVENTORY: `
<div class="inv_item">
  <img src="{{src}}" title="{{name}}" alt="{{name}}" class="item-image">
  <div class="item-description">
    <h3>{{name}}</h3>
    <p>{{description}}</p>
    <div>
      <p><strong>Нашедший:</strong> {{userName}} (ID: {{userId}})</p>
      <p><strong>Страница:</strong> <a href="{{pageUrl}}" target="_blank">{{topicSubject}}</a></p>
      <p><strong>Время находки:</strong> {{foundTime}}</p>
    </div>
  </div>

<span class="pulse-donate"
  data-user="${UserLogin}"
  data-userid="${UserID}"
  data-topic="${document.title || ''}"
  data-url="${location.href}"
  data-time="${new Date().toLocaleString('ru-RU')}"
  data-item="${itemName}"
  data-qty="1"
  data-key="${UserID}|${itemName}|${Date.now()}|${Math.random().toString(16).slice(2)}"
  style="display:none"></span>

</div>
`,


    	ALERTS: {
        SUCCESS: `Ты подобрал ингредиент "{{itemName}}"`,
        TOO_EARLY: `Стоило вам на миг отвернуться, и предмет исчез так, будто его никогда не было здесь.`, // таймаут не прошёл
        ERROR: `Ошибка при добавлении предмета`
    	}
        };
    
// Использование
$(document).ready(function() {

const ril_ALLOWED = [1, 2, 6]; // Группы, которые имеют право участвовать в акции
	if(ril_ALLOWED.indexOf(GroupID) == -1) return;

	const USE_ALEX_NOTIFICATIONS = true; // Интеграция с уведомлениями от Алекса
	const FROM_ID = 1; // От id какого акка отправляется уведомление (подставится в ссылку) 
	const FROM_USERNAME = 'SYSTEM'; // От какого имени отправляется уведомление (подставится в ссылку) 
	
	if(USE_ALEX_NOTIFICATIONS && typeof notifications != 'undefined') {
    notifications.addTemplate('ril_notif', {
    	title: 'Получение предмета',
    	url: '/viewtopic.php?pid={PID}#p{PID}',
    	html: `<span>Предмет '<strong>{ITEM_NAME}</strong>' добавлен в Ваш <a href=\"/viewtopic.php?pid={PID}#p{PID}\">Инвентарь</a><br /></span>`,
    	description: 'Оповещать о добавлении предметов в инвентарь.'
    });
	}
	
	if(window.location.href.indexOf("viewtopic") > -1 || window.location.href.indexOf("edit.php") > -1) {

    const imageLoader = new RandomImageLoader(
    	0.9, // Вероятность выпадения на странице
    	'https://forumstatic.ru/files/001c/84/76/52735.txt?v=2', // Файл с картинками и т.п.
    	0, // Минимум МИНУТ между появлением предметов
    	'21', // Топик, куда выкладывается результат
    	ril_TMPL, // Шаблоны сообщений
    	USE_ALEX_NOTIFICATIONS,
    	FROM_ID,
    	FROM_USERNAME,
    	false // Включить отладочный вывод
    );
    imageLoader.init();
	}
});
</script>
<style>
/* 1. Определяем анимацию с помощью drop-shadow */
@keyframes pulse-contour-glow {
  0% {
    /* Начало: слабое свечение */
    filter: drop-shadow(0 0 3px rgba(255, 255, 100, 0.4)); /* Меньший радиус */
  }
  50% {
    /* Середина: максимальное свечение */
    filter: drop-shadow(0 0 10px rgba(255, 255, 100, 0.9)) 
            drop-shadow(0 0 15px rgba(255, 255, 100, 0.5)); /* Более интенсивное и широкое свечение */
  }
  100% {
    /* Конец: возвращаемся к начальному слабому свечению */
    filter: drop-shadow(0 0 3px rgba(255, 255, 100, 0.4));
  }
}

/* 2. Применяем анимацию к классу glow-image */
.glow-image {
  /* Применяем анимацию: 2 секунды, бесконечно, туда-обратно */
  animation: pulse-contour-glow 2s infinite alternate; 
  /* Важно: filter: drop-shadow() заменил box-shadow */
}
</style>
<script src="https://forumstatic.ru/files/001c/52/b6/39259.js"></script>
