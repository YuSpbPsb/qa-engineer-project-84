
Alexander Zaytsev 20 марта, 14:46
Привет, Юрий!

Поздравляю с началом первого проекта, давай приступим к проверке!

    Общие проблемы

    https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L7 - В поле прекондишена должна быть указана ТОЛЬКО нужная и необходимая информация. Мы не заполняем и не тратим время на поле только для того чтобы что то написать.#+

Информация вроде "Открыта страница Магазин" абсолютно никак не помогает в прохождении кейса - это НЕ обязательное условие и не условие при отсутствии которого проверяющий не сможет понять что ему делать дальше. Давай удалим такое ВЕЗДЕ#+

    https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L3 - давай уберем везде из назхваний слово "Возможности" проверка это факт а не возможностей)#+]
###############++


test-cases.yml
1#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L14 - очень дотошно описываешь ОР, с одной стороны ты молодец что так серьезно подходишь к этому вопросу)

НО - это будет отнимать у тебя время в будущем - в реальных условиях) Поэтому можно не выводить все так аккуратно в плане окончаний и красивых слов)

Отображаются товары согласно введенного запроса - вот и все)
2#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L27 - тоже самое что и выше

Отображаются товары выбранного бренда

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L17 - у тебя говорится про категории а выбираешь ты бренды исправляем название
3#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L41 - сделать самостоятельно по примеру выше
4#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L55 - у нас по умолчанию чек бокс всегда включен - поэтому если я сейчас пойду по твоему шагу я выключу чек бокс и тогда ОР не соотвествует тому что я увижу

Потому что отключенный чек бокс должен показать "Все товары незаивисимо в наличии они или нет"#?
5#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L69 - исправить согласно примерам выше
6#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L72 - а мы и без кейса постоянно открываем главную писать на такое не нужно - удаляем
7#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L85 - Проверка открытия карточки товара

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L95 - Открыта карточка товара с подробным описанием
8#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L106 - не надо давать двусмысленные шаги) Важно четко следовать тому сколько раз нажать ведь от этого будет зависеть конечный результат

"Выбрать любой товар" "Добавить выбранный товар в корзину"

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L108 - я прочитал кейс и понял что он не соотвествует названию

Ты проверяешь "Появление бейджа с количеством товара на иконке корзины"
9#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L111 - а вот это "Проверка добавления товара в корзину"
10#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L140 - проверка смены языка на русский
11#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L191 - ты слишком увлекаешься прекондишенами)

У тебя кейс состоит из одного шага - зачем такие сложные прекондишены когда мы можем в шагах все это корректно и четко описать?

Прекондишен хорошо чтобы не перегружать и так большие кейсы - а если у тебя шаг из одного шага - это усложняет читаемость таких кейсов

Давай выведем в шаги
12#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L202 - тоже самое что и выше
13#+

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/test-cases.yml#L229 - то же самое что и выше#+
####################
bugreports.yml

Давай добавим еще 3 новых баг репорта - и вот одна подсказка к одному из них: Попробуем оформить заказ с включенным девтулз - возможно ты найдешь интересную ошибку!
1

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/bugreports.yml#L3 - Нет мобильной версии
#+
Все проще проще и проще)

https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/bugreports.yml#L9 - Есть мобильная версия сайта
#+
https://github.com/YuSpbPsb/qa-engineer-project-84/blob/d39c424cf38f05dbde923a7c5a8769a458d404d5/bugreports.yml#L12 - нет мобильной версии сайта
#+
все проще и еще проще)
testing-report.yml

Актуализировать и изменить в соотвествии с изменениями и указаниями выше.
regress-report.yml

Актуализировать и изменить в соотвествии с изменениями и указаниями выше.
