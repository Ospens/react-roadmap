+++
title = 'Крестики-нолики'
weight = 3
+++

# Крестики-нолики

## О проекте

**[Правила](https://ru.wikipedia.org/wiki/%D0%9A%D1%80%D0%B5%D1%81%D1%82%D0%B8%D0%BA%D0%B8-%D0%BD%D0%BE%D0%BB%D0%B8%D0%BA%D0%B8)**, если вдруг кто-то не знает

## Чему научишься

Этот урок объединяет в себе два предыдущих. Здесь мы

- Закрепим работу с HTML/CSS
- Научимся осмысленно именовать классы
- Научимся создавать элементы и манипулировать ими посредством JavaScript.
- Настроим и освоим инструмент для автоматического форматирования кода - prettier. Он широко распространен в нашей работе и помогает писать унифицированный код. В нем очень мало настроек, из-за чего код на выходе, визуально, получается примерно одинаковым между различными проектами. Поработав некоторые время с форматтером, вы поймете, что чужой код с prettier читается гораздо легче.

## Материалы для подготовки


> Список материалов может меняться время от времени. Самостоятельный поиск других источников приветствуется

- [БЭМ](https://ru.bem.info/methodology/) документация
- [https://timeweb.cloud/tutorials/javascript/kak-dobavit-javascript-v-html](https://timeweb.cloud/tutorials/javascript/kak-dobavit-javascript-v-html)
- [https://learn.javascript.ru/](https://learn.javascript.ru/). **Часть 2. Браузер: документ, события, интерфейсы.** 1-4 пункты
- [https://doka.guide/js/dom/](https://doka.guide/js/dom/)
- [https://doka.guide/js/forms/](https://doka.guide/js/forms/)
- **Prettier**
    1. Теория. [https://habr.com/ru/companies/ruvds/articles/428173/](https://habr.com/ru/companies/ruvds/articles/428173/). Нам интересен только блок с Prettier. Остальное материал со звездочкой, к нему вернемся позже.
    2. Устанавливаем node.js: [https://nodejs.org/en](https://nodejs.org/en)
    3. Гайд для VS Code: [https://www.digitalocean.com/community/tutorials/how-to-format-code-with-prettier-in-visual-studio-code-ru](https://www.digitalocean.com/community/tutorials/how-to-format-code-with-prettier-in-visual-studio-code-ru)
    4. Гайд для WebStorm: [https://www.jetbrains.com/help/webstorm/prettier.html#ws_prettier_reformat_code](https://www.jetbrains.com/help/webstorm/prettier.html#ws_prettier_reformat_code)
    5. На данном этапе горячо рекомендую включить **форматирование при сохранении** в редакторе кода, чтобы не забывать форматировать код вручную.
- [https://scand.com/ru/company/blog/functional-programming-vs-oop/](https://scand.com/ru/company/blog/functional-programming-vs-oop/)
- Материалы из [[Парсер акций]]

## Техническое задание

Макет приложения

https://www.figma.com/design/IM6ajWNLVgyMi6Ou4dObs0/Tic-Tac-Toe-(Interactive-component)-(Community)-(Copy)?node-id=5-252&t=6sYSDAVGiVmwMbOw-1

В правом верхнем углу есть кнопка, по нажатию на которую можно запустить интерактивный макет.

![[/Untitled 45.png|Untitled 45.png]]



1. CSS классы должны быть названы в соответствии с [БЭМ](https://ru.bem.info/methodology/) методологией.
2. Допускается выбор нескольких одинаковых элементов подряд.
3. При наведении на пустую клетку происходит анимация: контур клетки пропадает и на его месте появляются два элемента: Крестик и Нолик
    1. При появлении элементы должны разъезжаться из центра клетки
    2. Когда курсор уходит с клетки - анимации должны проиграться в обратном порядке
    3. Если выбран Крестик и Нолик, то на месте пустой клетки должен появиться выбранный элемент. При уходе курсора с клетки не должно ничего происходить. При нажатии на уже выбранный элемент не должно ничего происходить
4. При победе крестиков - линия красная
5. При победе ноликов - линия зеленая
6. Если не получается создать линии из двух пунктов выше посредством CSS - допускается экспортировать их и использовать как SVG картинки.

## Заметки

1. Рекомендую начать с верстки. Сначала сделать статически HTML/CSS элементы, а после этого добавлять к ним JS с логикой.
2. Для удобного поиска элементов можно задать им специфичные классы, а после использовать [https://developer.mozilla.org/ru/docs/Web/API/Document/querySelector](https://developer.mozilla.org/ru/docs/Web/API/Document/querySelector) для выбора нужного элемента

## Обратная связь и контакты

По любым вопросам пиши мне, [@i_urKing](https://t.me/i_urKing), и подписывайся на мой канал [@js_is_easy](https://t.me/+jsgZ3_UEcoBlNjgy)
