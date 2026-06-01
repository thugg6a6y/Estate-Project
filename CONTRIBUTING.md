# Участь у проєкті

## Git Flow

1. Оновіть `develop`: `git checkout develop && git pull`
2. Створіть гілку від `develop`:
   ```bash
   git checkout -b feature/hero
   ```
3. Працюйте лише у відповідних файлах секції (див. таблицю нижче).
4. Комітьте змістовні повідомлення (українською або англійською):
   - `feat(hero): додано блок статистики`
   - `fix(header): вирівняно навігацію на планшеті`
5. Відкрийте **Pull Request** у `develop`, опишіть зміни та додайте скріншот.
6. Після рев’ю — merge. Реліз на `main` — окремим PR з `develop`.

## Мапінг гілок і файлів

| Гілка | HTML (секція в `index.html`) | CSS |
|--------|------------------------------|-----|
| `feature/header` | `<header class="site-header">` | `css/sections/header.css` |
| `feature/hero` | `.hero` | `css/sections/hero.css` |
| `feature/services` | `.services` | `css/sections/services.css` |
| `feature/properties` | `#properties` | `css/sections/properties.css` |
| `feature/testimonials` | `#testimonials` | `css/sections/testimonials.css` |
| `feature/faq` | `#faq` | `css/sections/faq.css` |
| `feature/cta` | `.cta` | `css/sections/cta.css` |
| `feature/footer` | `.site-footer` | `css/sections/footer.css` |

Спільні стилі (`css/base/`, `css/components/`) змінювати в окремій гілці `feature/design-system` з узгодженням.

## Стандарти коду

- Семантичні теги: `header`, `nav`, `main`, `section`, `article`, `figure`, `footer`
- BEM-подібний неймінг: `block__element`, модифікатор `block--modifier`
- Без інлайн-стилів; кольори лише через CSS-змінні з `variables.css`
- Відступи з шкали Figma (`--space-*`)
- Перед PR: перевірити HTML/CSS у W3C Validator

## Заборона

Не копіювати готові шаблони з інших репозиторіїв. Усі рішення — власна верстка в рамках макету Figma.
