# Hadzhalov Estate

Головна сторінка агенції нерухомості (верстка за макетом [Estatein — Produce UI, dark theme](https://www.figma.com/design/ZtzhjF1nEqnZWJqMqlenbx/Real-Estate-Business-Website-UI-Template---Dark-Theme-%7C-Produce-UI--Community-)).

## Структура проєкту

```
estatein/
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

## Локальний запуск

Відкрийте `index.html` у браузері або через локальний сервер:

```bash
cd estatein
python3 -m http.server 8080
# http://localhost:8080
```

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
