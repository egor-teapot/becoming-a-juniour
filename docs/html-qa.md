# HTML вопрос - ответ

### Какие семантические теги используются для верстки таблиц?
caption, thead, tbody, tfooter

<br>

### По нажатию на ссылку как открыть ее на новой странице?
```html
<a target="_blank"></a>
```

<br>

### Как выбрать checkbox или radiobutton по умолчанию?
```html
<input type="checkbox" checked></input>
<input type="radio" checked></input>
```
<br>

### Для чего используется атрибут name для тега input?
При отправки данных на бэкэнд name используется для обозначения
названия данных.

```html
<input name="email" type="email">
<input name="password" type="password">
```

данные получаемые на бэкэнде
```json
{"email": "some-email@dom.com", "password": "12791230"}
```

<br>

### Как реализовать элемент следующего вида?
<fieldset>
<legend>Header</legend>
<p>Some text, some text, some text, some text, some text, some text</p>
</fieldset>

<br>

```html
<legend>Header</legend>
<p>Some text, some text, some text, some text, some text, some text</p>
```

<br>

### Как зделать поле обязательным для заполнения?
Для этого используется required

```html
<input type="password" required>
```

<br>

### Как возможно реализовать кнопку для оформления?
Кнопку для отправки можно реализовать используя

```html
<input type="submit">
```

или

```html
<button type="submit">Submit</button>
```

<br>

### Какие значения может принемать type в input?
- text
- password
- email
- checkbox
- radio
- reset
- submit
- tel
- number
- range
- search
- file

<br>

### Для чего используется action в форме?
Атрибут action определяет каким http методом будут посланы
данные на сервер. Как правило используется "POST" а не "GET"
так как он безопаснее.

<br>

### 