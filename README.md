## TODO

### High Priority

### Low Priority

# My Project

This is a sample project that demonstrates basics of HTML and CSS, based on BEM approach.
See \*.css files in common.blocks folder.

Files structure:

```
.
├── README.md
├── checklist-1.pdf
├── common.blocks --> CSS block files according to BEM
│   ├── description.css
│   ├── digits.css
│   ├── feynman.css
│   ├── footer.css
│   ├── header.css
│   ├── kaufman.css
│   ├── logo.css
│   ├── page.css
│   ├── section-subtitle.css
│   ├── section-title.css
│   ├── table.css
│   └── two-columns.css
│  
├── images
│   ├── facebook_color_white.svg
│   ├── feynman.png
│   ├── instagram_color_white.svg
│   ├── kaufman-triangle.svg
│   ├── logo_place_footer.svg
│   ├── logo_place_header.svg
│   ├── two_again.png
│   └── vk_color_white.svg
├── index.html
├── styles
│   ├── normalize.css
│   └── style.css --> not used
├── texts.md
└── tree.md
```

## Getting Started

Use git clone to get copy of the project.

### Prerequisites

Live server vscode extension to run project locally.
EditorConfig vscode extension to format code. See .editorconfig

### Installing

Step by step instructions on how to install the project

1. Clone the repository
2. Start the server

## Usage

open 127.0.0.1 port 5500 locally

## Contributing

None

## License

This project is licensed under the MIT License

## Contact

- Email: dev.miroshnikov.m@ya.ru

## Commments

"БЭМ не рекомендует общие ресеты.
Блок — независимый от окружения компонент. Он не может рассчитывать на то, что стили сброшены какими-то внешними по отношению к блоку средствами"

You should reset CSS on block level.

Page structure:

Pseudocode:

```
div class="page"
  header class="header" -> reset CSS
  main class="content
    section class="digits -> reset CSS
    section class="feynman" -> reset CSS
    section class="kaufman" -> reset CSS
  footer class="footer" -> reset CSS
```

reset CSS:

```
  margin: 0;
  padding: 0;
  border-box - надо указывать?

```

# Checklist

## Общее

- [x] Репозиторий содержит все необходимые файлы: изображения, файлы стилей и HTML?
- [x] Стили подключены отдельным файлом? Подключён ли в head файл normalize.css ?
- [x] Соответствует ли вёрстка брифу внешне?
- [x] В коде HTML и CSS нет опечаток? Страница валидна? Рекомендуем использовать валидатор разметки от w3.org
- [x] Все блоки из брифа свёрстаны?
- [x] Все блоки, элементы и модификаторы названы в соответствии с брифом?
- [x] Названия классов CSS в разметке соответствуют явно указанным в брифе?
- [x] Добавлены ли в футер иконки и текст?
- [x] В футере есть ссылки? По ним можно кликнуть?

## Семантика

- [x] У всех изображений есть атрибут alt ?
- [x] Для вёрстки заголовков применяются несколько тегов от h1 до h6 , текстовые блоки размечены тегами
      p, присутствуют элементы header, main, footer, section? Они используются по назначению?

## Заголовки

- [x] На странице есть заголовок первого уровня? Соответствуют ли заголовки иерархии страницы? Нет ли на странице скрытых с помощью CSS заголовков?

## CSS

- [x] Соответствуют ли брифу значения отступов у элементов?
- [x] Обнулены ли стандартные значения отступов у элементов (заголовков, параграфов, списков) в соответствии с брифом?
- [x] Картинки в проекте не перекрывают текст? Текст располагается над изображением по оси Z?
- [x] Абсолютное позиционирование применено только к тем элементам, о которых сказано в брифе?
- [x] У всех ли абсолютно спозиционированных элементов заданы координаты по двум осям (например, top и left )?
- [x] У блоков фиксированная высота? Растягивается ли блок, когда текст внутри него увеличивается в 2–3 раза?
- [x] Ссылки, фоны секций и шрифты раскрашены как в брифе?
- [x] Для создания сеток используется flex либо grid-layout ? - используется flex

Смотри, мы в ПР должны придерживаться БЭМ Nested. Соответственно, у нас не должно быть папок common.blocks/ и styles, а также файла styles.css. В файлах блоков (<block-name>.css) должны быть только стили блоков, а стили элементов и/или модификаторов - в соответствующих подпапках.
Что надо сделать:

1. Переименуй common.blocks/ в blocks.
2. Внутри blocks создай по папке для каждого блока.
3. В каждой папке блока надо создать подпапки для элементов и модификаторов блока, в них поместить CSS-файлы элементов и модификаторов блока. Если у элементов есть модификаторы - создаём для них подпапки уже внутри подпапки элемента, и кладём туда CSS-файл со стилями модификатора элемента.
4. Создаём папку vendor/, в ней подпапку fonts/, в последнюю складываем файлы шрифтов, в самой vendor/ должен лежать normalize.css. Там же создаём файл fonts.css с подключением всех шрифтов (@font-face ...).
5. Создаём папку pages/, в ней файл index.css и в нём подключаем с помощью @import url(...) сначала normalize.css, потом fonts.css, и после все блоки, элементы и модификаторы из папки blocks/. Надо следить за тем, чтобы элементы импортировались после своего блока, а модификаторы - ПОСЛЕ (НИЖЕ) модифицируемого блока или элемента. Последнее - особенно важно, или работать не будет :)
6. В index.html в <head> подключаем index.css через <link rel="stylesheet" ...>
7. Проходимся по всем HTML- и CSS-файлам, и проверяем везде пути, корректируем в соответствии с новой структурой файлов и папок :)

Или у вас ещё БЭМ не было?
Тогда смотри readme.md или пиши все стили кучей в styles.css
А простыня выше пригодится при выполнении ПР2 :)
