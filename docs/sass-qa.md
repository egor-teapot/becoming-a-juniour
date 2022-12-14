# Sass вопрос-ответ

<br>

## Как создать переменную
```
$name-of-var: value
```
Переменные создаются вне применяемых стилей

<br>

## Как создать тип данных с структурой ключ-значение
```
$font-weights: (
    "regular": 400,
    "medium": 500,
    "bold": 700
)
```

чтобы обратится к одному из значений необходимо использовать map-get()
```
font-weight: mag-get($font-weights, bold)
```

<br>

## Как работает вложенность в sass
Sass позволяет обращатся к элементам страницы
Как будто бы мы писати в парадигме ООП

sass
```
.main
    margin: 0 auto
    width: 80%
    background: gray

    #{&}-section
        font-size: 1.2rem
    
        &:hover
            color: pink
```

css
```
.main {
    margin: 0 auto
    width: 80%
    background: gray
}

main main-section {
    font-size: 1.2rem
}

main main-section:hover {
    color: pink
}
```
Это позволяет сделать написание стилей
более структурированным

<br>

## Как импортировать один sass в другой
```
@import './sass-file'
```

## как сделать так чтобы sass файл не распозновался транслятором
В начале названия sass файла поставить "_" например
```
_varaibles.sass
_reset.sass
```
такие файлы не будут компилироватся в .css файлы