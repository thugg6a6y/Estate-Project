# Hadzhalov Estate

Головна сторінка агенції нерухомості (верстка за макетом [Estatein — Produce UI, dark theme](https://www.figma.com/design/ZtzhjF1nEqnZWJqMqlenbx/Real-Estate-Business-Website-UI-Template---Dark-Theme-%7C-Produce-UI--Community-)).
## Опис проєкту

Hadzhalov Estate — це односторінковий сайт (landing page) агенції нерухомості в Києві. На головній сторінці представлені преміальні житлові комплекси: Tetris Hall, Manhattan City, Taryan Towers та Time. Сайт виконаний у темній темі за макетом Figma (шаблон Estatein від Produce UI) і містить основні блоки: шапку з навігацією, hero-секцію, послуги, каталог ЖК з описами та цінами, відгуки клієнтів, блок FAQ, заклик до дії та підвал з формою підписки та посиланнями. Інтерфейс українською мовою.

## Технології

HTML5 — семантична розмітка (header, nav, main, section, article, footer тощо)
CSS3 — верстка без фреймворків; модульна структура стилів (базові стилі, компоненти, окремі файли для кожної секції)
CSS-змінні (custom properties) — кольори, відступи та типографіка з макету Figma
Google Fonts (Urbanist) — шрифт з макету
Git / Git Flow — гілки main, develop, feature/* для роботи по секціях та pull request’и
Локальні зображення (PNG) — візуалізації житлових комплексів у папці assets

## Структура проєкту

```
estate/
├── index.html              # Семантична розмітка сторінки
├── css/
│   ├── main.css            # Точка входу (імпорти модулів)
│   ├── base/               # Токени, reset, типографіка, layout
│   ├── components/         # Кнопки, лого, картки, пагінація
│   └── sections/           # Стилі окремих секцій (1 файл = 1 секція)
├── assets/                 # Зображення ЖК
├── docs/
│   ├── GITFLOW.md          # Git Flow та гілки
│   └── VALIDATION.md       # Перевірка валідності
└── CONTRIBUTING.md
```

## Запуск сайту

Відкрийте https://thugg6a6y.github.io/Estate-Project/

## Дизайн-система (Figma)

| Токен | Значення |
|--------|----------|
| Фон сторінки | `#141414` |
| Фон карток | `#1A1A1A` |
| Бордер | `#262626` |
| Акцент | `#703BF7` |
| Текст вторинний | `#999999` |
| Шрифт | Urbanist |
| Контейнер | max 1296px, padding до 162px |

## Git Flow

- `main` — стабільна версія для здачі / продакшену
- `develop` — інтеграційна гілка
- `feature/<секція>` — одна секція = одна гілка → Pull Request у `develop`

Детальніше: [docs/GITFLOW.md](docs/GITFLOW.md)

## Валідність

Перевірка HTML: [validator.w3.org](https://validator.w3.org/#validate_by_upload)  
Перевірка CSS: [jigsaw.w3.org/css-validator](https://jigsaw.w3.org/css-validator/)

Інструкція: [docs/VALIDATION.md](docs/VALIDATION.md)

## Браузери

Chrome, Firefox, Edge (останні версії).
