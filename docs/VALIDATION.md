# Перевірка валідності HTML і CSS

## HTML

1. Відкрийте [W3C Markup Validator](https://validator.w3.org/#validate_by_upload)
2. Завантажте файл `index.html` з кореня проєкту
3. Переконайтеся, що немає **Errors** (попередження Info/Warning допустимі, якщо обґрунтовані)

Або через URI (якщо сайт опублікований):

```
https://validator.w3.org/nu/?doc=https://your-domain.com/
```

## CSS

1. [W3C CSS Validator](https://jigsaw.w3.org/css-validator/)
2. Перевіряйте файли по черзі: `css/main.css` та модулі в `css/base/`, `css/components/`, `css/sections/`
3. Режим **CSS Level 3**

Примітка: `@import` у `main.css` — валідний CSS; валідатор перевіряє імпортовані файли при повній перевірці з кореня.

## Локально (опційно)

```bash
# macOS — встановити tidy, якщо потрібно: brew install tidy-html5
tidy -e -q index.html
```

## Чеклист перед PR

- [ ] `lang="uk"` на `<html>`
- [ ] Один `<h1>`, ієрархія заголовків без пропусків
- [ ] Усі `<img>` мають `alt`
- [ ] Форми з `<label>` (видимий або `.visually-hidden`)
- [ ] Інтерактивні елементи доступні з клавіатури (`:focus-visible`)
