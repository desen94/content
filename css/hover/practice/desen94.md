🛠 Состояние `:hover` удобно использовать в [медиавыражениях](/css/media) по характеристикам взаимодействия. Пример исключающий тач-устройства:

```css
.link {
  color: #ffffff;
  text-decoration-color: #ffd829;
  transition: color 0.5s;
}

@media (any-hover: hover) { /* есть возможность навести указатель на элемент */
  .link:hover {
    color: #ed6742;
    transition: color 0.1s;
  }
}
```

<iframe title="Ховер-эффект в медиавыражении" src="../demos/link-hover-media/" height="220"></iframe>

Стоит заметить, что характеристика `any-hover: hover` включает в себя и touch-устройства, но только если к ним подключено устройство ввода с нужным функционалом (мышь, тачпад и т.п.).

По аналогии можно использовать и другие состояния [`:link`](/css/link), [`:visited`](/css/visited), [`:active`](/css/active).
