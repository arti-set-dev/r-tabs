# graph-tabs
---
## Описание плагина

Простой и доступный плагин табов с возможностью изменения некоторых параметров

Демо: https://codepen.io/arti-set-dev/pen/YzjMdJx

## Загрузка и инициализация

Для загрузки введите команду: `npm i r-tabs`.

После загрузки перед инициализацией напишите базовую html разметку для работы плагина. Она должна выглядеть следующим образом:
```html 
<div class="tabs" data-tabs="tab1">
    <ul class="tabs__nav">
      <li class="tabs__nav-item"><button class="tabs__nav-btn" type="button">Один</button></li>
      <li class="tabs__nav-item"><button class="tabs__nav-btn" type="button">Два</button></li>
      <li class="tabs__nav-item"><button class="tabs__nav-btn" type="button">Три</button></li>
    </ul>
    <div class="tabs__content">
      <div class="tabs__panel">Один контент</div>
      <div class="tabs__panel">Два контент</div>
      <div class="tabs__panel">Три контент</div>
    </div>
  </div>
  <div class="tabs" data-tabs="tab2">
    <ul class="tabs__nav">
      <li class="tabs__nav-item"><button class="tabs__nav-btn" type="button">Один</button></li>
      <li class="tabs__nav-item"><button class="tabs__nav-btn" type="button">Два</button></li>
      <li class="tabs__nav-item"><button class="tabs__nav-btn" type="button">Три</button></li>
    </ul>
    <div class="tabs__content">
      <div class="tabs__panel">Один контент</div>
      <div class="tabs__panel">Два контент</div>
      <div class="tabs__panel">Три контент</div>
    </div>
  </div>
```


Для инициализации пропишите следующий код: 
```js
const tabs = new GraphTabs('tab1');
```
## Настройки

### vertical

Данный параметр отвечает за ориентацию табов. По умолчанию ориентация горизонтальная. Для изменения ориентации пропишите параметр `vertical` со значением `true`.

```js
const tabs = new GraphTabs('tab1', {
  vertical: true,
});
```