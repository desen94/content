🛠 Состояние `:hover` удобно задавать внутри [медиавыражений](/css/media) с условием по типу взаимодействия с устройством. Пример, исключающий тач-устройства:

```css
.link {
  color: #ffffff;
  text-decoration-color: #ffd829;
  transition: color 0.5s;
}

/* Есть возможность навести указатель на элемент */
@media (any-hover: hover) {
  .link:hover {
    color: #ed6742;
    transition: color 0.1s;
  }
}
```

<iframe title="Ховер-эффект в медиавыражении" src="../demos/link-hover-media/" height="220"></iframe>

> Условие `any-hover: hover` может допускать тач-устройства, но только если к ним подключено устройство ввода с нужной функциональностью (мышь, тачпад и т. п.)

По аналогии можно использовать и другие состояния — [`:link`](/css/link), [`:visited`](/css/visited), [`:active`](/css/active).
