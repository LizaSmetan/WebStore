Web Store
=====================

### Файлы папки app

Название файла  | Содержание файла
----------------|----------------------
index.html      | Главная страница сайта
category.html   | Страница со списком продуктов
product.html    | Страница с описанием продукта

**Файлы папки app/css**

Название файла                    | Содержание файла
----------------------------------|----------------------------------
css/bootstrap.css                 | Подключенные стили Bootstrap 3
css/flexslider.css                | Стили карусели на странице с описанием продукта
css/font-awesome.css              | Иконки Font-awesome
css/fonts.css                     | Шрифты
css/jquery.formstyler.theme.css   | Стили формы количества товара JQuery
css/slicknav.css                  | Стили мобильного меню
css/sprite.css                    | Сконвертированные иконки
css/style.css                     | Основные стили

**Файлы папки app/js**

Название файла               | Содержание файла
-----------------------------|-----------------------------
js/bootstrap.min.js          | Подключенные плагины Bootstrap 3
js/jquery.flexslider-min.js  | Плагины карусели на странице с описанием продукта
js/jquery.formstyler.min.js  | Плагины формы количества товара JQuery
js/jquery.slicknav.min.js    | Плагины мобильного меню
js/plugins.min.js            | Основные плагины

---
**Используемые шрифты и начертания**

1. Harmonia:
 1)black;
 2)regular;
 3)semibold;
 4)bold;
 5)italic;
2. Font-awesome.
---

***Внешние плагины***
    [JQuery-ui](https://code.jquery.com/ui/1.12.1/themes/base/jquery-ui.css)

---

**Стандартные классы**

'''css

.flex-container{     /* Для блоков с елементами, выстроеными в ряд */
	display: flex;
}
.align-center{      /* Выравнивание елементов по центру относительно флекс-контейнера */
	align-items: center;
}
.justify-sp-between{     /* Блоки распределены вдоль главной оси флекс-контейнера, при этом первый элемент прижат к началу оси, а последний - к концу */
	justify-content: space-between;
}
.flex-wrap{         /* Для переноса елементов флекс-контейнера при нехватке места */
	flex-wrap: wrap;
}
.orange-text{     /* Оранжевый цвет текста */
	color: #ff5912;
}
.light-grey-text{    /* Светло-серый цвет текста */
	color: #e3e6ea;
}
.red-bg{         /* Красный фон */
	background-color: #e12e3f;
}
.black-bg{             /* Черный фон */
	background-color: #34404b;
}
.blue-bg{          /* Синий фон */
	background-color: #3ab3ff;
}
.green-bg{       /* Зеленый фон */
	background-color: #2fd967;
}
.white-bg{          /* Белый фон */
	background-color: #fff;
}
.light-orange-bg{            /* Светло-оранжевый фон */
	background-color: #ff9060;
}
.orange-bg{       /* Оранжевый фон */
	background-color: #ff5912;
}
'''

**Плагины**

'''js

$( function(){

	var sidebar_btn = $(".mobile-sidebar-btn");  // Вводим переменную sidebar_btn
	var main = $("main");      // Вводим переменную main 
	var overlay = $(".overlay");   // Вводим переменную overlay 

	sidebar_btn.on("click", function(e) {  // Создаем функцию для добавления переменной main класса show при клике на кнопку
		main.toggleClass("show");
	});
	
	overlay.on("click", function(e) {   // Создаем функцию для снятия с переменной main класса show при клике на overlay
		main.toggleClass("show");
	});

});

'''