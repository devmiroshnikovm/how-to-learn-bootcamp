## TODO

### High Priority

- [ ] check review errors

### Low Priority

# My Project

This is a sample project that demonstrates basics of HTML and CSS, based on BEM approach.

Files structure:

```
.
├── README.md
├── blocks
│   ├── cards
│   │   ├── __description
│   │   │   └── cards__description.css
│   │   ├── __image
│   │   │   └── cards__image.css
│   │   ├── __item
│   │   │   └── cards__item.css
│   │   ├── __title
│   │   │   └── cards__title.css
│   │   └── cards.css
│   ├── content
│   │   └── content.css
│   ├── description
│   │   └── description.css
│   ├── digits
│   │   ├── __section-subtitle
│   │   │   └── digits__section-subtitle.css
│   │   ├── __section-title
│   │   │   └── digits__section-title.css
│   │   ├── __table-cell
│   │   │   └── digits__table-cell.css
│   │   └── digits.css
│   ├── feynman
│   │   ├── __link
│   │   │   └── feynman__link.css
│   │   ├── __main-illustration
│   │   │   └── feynman__main-illustration.css
│   │   ├── __subtitle
│   │   │   └── feynman__subtitle.css
│   │   ├── __title
│   │   │   └── feynman__title.css
│   │   └── feynman.css
│   ├── footer
│   │   ├── __author
│   │   │   └── footer__author.css
│   │   ├── __column
│   │   │   ├── footer__column.css
│   │   │   ├── footer__column_content_copyright.css
│   │   │   ├── footer__column_content_info.css
│   │   │   └── footer__column_content_social.css
│   │   ├── __column-heading
│   │   │   └── footer__column-heading.css
│   │   ├── __column-link
│   │   │   └── footer__column-link.css
│   │   ├── __column-links
│   │   │   └── footer__column-links.css
│   │   ├── __columns
│   │   │   └── footer__columns.css
│   │   ├── __social-icon
│   │   │   └── footer__social-icon.css
│   │   └── footer.css
│   ├── header
│   │   ├── __link
│   │   │   └── header__link.css
│   │   ├── __main-illustration
│   │   │   └── header__main-illustration.css
│   │   ├── __square-pic
│   │   │   └── header__square-pic.css
│   │   ├── __subtitle
│   │   │   └── header__subtitle.css
│   │   ├── __title
│   │   │   └── header__title.css
│   │   └── header.css
│   ├── kaufman
│   │   ├── __table-cell
│   │   │   └── __table-cell.css
│   │   ├── __triangle
│   │   │   └── kaufman__triangle.css
│   │   └── kaufman.css
│   ├── khan
│   │   ├── __author
│   │   │   └── khan__author.css
│   │   ├── __book-container
│   │   │   └── khan__book-container.css
│   │   ├── __book-pic
│   │   │   └── khan__book-pic.css
│   │   ├── __buy-link
│   │   │   └── khan__buy-link.css
│   │   ├── __container
│   │   │   └── khan__container.css
│   │   ├── __quote
│   │   │   └── khan__quote.css
│   │   ├── __quote-author
│   │   │   └── khan__quote-author.css
│   │   ├── __quote-author-subline
│   │   │   └── khan__quote-author-subline.css
│   │   ├── __title
│   │   │   └── khan__title.css
│   │   └── khan.css
│   ├── logo
│   │   ├── _place
│   │   │   ├── logo_place_footer.css
│   │   │   └── logo_place_header.css
│   │   └── logo.css
│   ├── oakley
│   │   └── oakley.css
│   ├── page
│   │   └── page.css
│   ├── resources
│   │   ├── __link
│   │   │   └── resources__link.css
│   │   ├── __logo-zone
│   │   │   └── resources__logo-zone.css
│   │   ├── __subtitle
│   │   │   └── resources__subtitle.css
│   │   ├── __title
│   │   │   └── resources__title.css
│   │   └── resources.css
│   ├── rotation
│   │   └── rotation.css
│   ├── section-subtitle
│   │   ├── section-subtitle.css
│   │   └── section-subtitle_theme_dark.css
│   ├── section-title
│   │   ├── section-title.css
│   │   └── section-title_theme_dark.css
│   ├── table
│   │   ├── __cell
│   │   │   └── table__cell.css
│   │   ├── __heading
│   │   │   ├── table__heading.css
│   │   │   └── table_heading_theme_dark.css
│   │   ├── __text
│   │   │   ├── table__text.css
│   │   │   └── table_text_theme_dark.css
│   │   └── table.css
│   ├── techniques
│   │   ├── __subtitle
│   │   │   └── techniques__subtitle.css
│   │   ├── __title
│   │   │   └── techniques__title.css
│   │   └── techniques.css
│   ├── two-columns
│   │   ├── __brief
│   │   │   └── two-columns__brief.css
│   │   ├── __main-text
│   │   │   └── two-columns__main-text.css
│   │   ├── __paragraph
│   │   │   └── two-columns__paragraph.css
│   │   ├── __span-accent
│   │   │   └── two-columns__span-accent.css
│   │   └── two-columns.css
│   └── video
│       ├── __iframe
│       │   └── video__iframe.css
│       ├── __iframes
│       │   └── video__iframes.css
│       ├── __subtitle
│       │   └── video__subtitle.css
│       ├── __title
│       │   └── video__title.css
│       └── video.css
├── build.js
├── images
│   ├── cards-attention.png
│   ├── cards-competence.png
│   ├── cards-interliving.png
│   ├── cards-question.png
│   ├── cards-recall.png
│   ├── facebook_color_white.svg
│   ├── feynman.png
│   ├── header-image.png
│   ├── instagram_color_white.svg
│   ├── kaufman-triangle.svg
│   ├── khan-book.jpg
│   ├── logo
│   │   ├── resources-arzamas.svg
│   │   ├── resources-n1.svg
│   │   ├── resources-polka.svg
│   │   └── resources-strelka.svg
│   ├── logo_place_footer.svg
│   ├── logo_place_header.svg
│   ├── tiktok-icon.svg
│   ├── two_again.png
│   ├── vk_color_white.svg
│   └── youtube-icon.svg
├── index.html
├── pages
│   └── index.css
├── technical specifications
│   ├── texts-brief1.md
│   ├── texts-brief2.md
│   └── texts.md
├── test.txt
├── tree.md
└── vendor
    └── normalize.css

79 directories, 111 files

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
