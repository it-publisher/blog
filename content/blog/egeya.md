---
title: "Эгея. Оформляем шапку блога"
date: 2024-02-11T20:41:15+05:00
slug: "egeya"
blogtags:
  - "веб"
  - "технодурка"
---

Разберем, как сделать навигационное меню в шапке блога.

## Что за «Эгея» такая?

«Эгея» это движок блога. Его придумал Илья Бирман.  
Вот официальный сайт <https://blogengine.ru/>

Прелесть этого движка в том, что он:

1. Бесплатный. Но есть платные фичи
2. [Легко устанавливается](https://antonkoshuba.ru/blog/all/install-egeya/)
3. Не требует глубоких знаний в вебе

Подробнее про «Эгею» можно посмотреть на ютубе [«Что делает движок блога „Эгея“ · Доклад, 2023»](https://youtu.be/vrcXLs_PhVA?si=GQZNbf_k-Pas7vKv)

## Зачем в блоге меню?

Если коротко — для навигации.

В шапке можно закрепить ссылки на разные теги, например, портфолио, фотографии, услуги, кейсы и что угодно еще. Или ссылку на сервис донатов, да, так тоже можно.

Вот несколько примеров:

<figure>
<img src="/blog/pictures/egeya-oformlyaem-shapku-bloga.png" alt="">
<img src="/blog/pictures/image.png" alt="">
<img src="/blog/pictures/egeya-oformlyaem-shapku-bloga-1.png" alt="">
<img src="/blog/pictures/egeya-oformlyaem-shapku-bloga-2.png" alt="">
<img src="/blog/pictures/egeya-oformlyaem-shapku-bloga-3.png" alt="">
</figure>

В таком виде шапка превращается в навигационное меню.

## Как сделать?

Вот что нужно будет сделать:

1. Выбрать нужные теги.
2. Оформить ХТМЛ-код.
3. Добавить код в настройки блога.

У вас всё получится. А если не получится, напишите мне, и я сделаю так, чтобы всё получилось.

### Выбираем теги

Для начала нужно определиться, какие теги добавить в шапку блога.  
Обычно все теги можно найти по адресу:

```
https://ваш_домен/blog/tags/
```

У меня адрес выглядит так:

<figure>
<img src="/blog/pictures/Snimok-ekrana-2024-02-11-v-20.03.40.png.jpg" alt="">
</figure>

Откройте страницы с нужными тегами. Нам понадобится их адрес.  
Пример:

```
https://antonkoshuba.ru/blog/tags/redaktura/
```

<figure>
<img src="/blog/pictures/Snimok-ekrana-2024-02-11-v-20.09.00.png.jpg" alt="">
</figure>

### Оформляем ХТМЛ-код

Чтобы меню было кликабельным, используем тег

```
<a href=""></a>
```

Пример:

```
<a href="адрес ссылки на тег">текст ссылки</a>
```

Наведем немного красоты. Зададим высоту блока ссылок, кегль и интерлиньяж, добавим неразрывные пробелы.

Вот мой пример:

```
<nav style= "height: 23.5px; font-size: 16px; line-height: 25.5px;"> &nbsp; <a href="https://antonkoshuba.ru/blog/tags/redaktura/">Редактура</a> &nbsp; <a href="https://antonkoshuba.ru/blog/tags/mir/">Мир</a> &nbsp; <a href="https://antonkoshuba.ru/blog/tags/portfolio/">Портфолио</a></nav>
```

Можете скопировать его, только не забудьте заменить ссылки на свои.

### Добавляем ХТМЛ-код в настройки

Нажмите на шестеренку:

<figure>
<img src="/blog/pictures/Snimok-ekrana-2024-02-11-v-20.11.38.png.jpg" alt="">
</figure>

Вставьте код из предыдущего шага в поле «Подзаголовок»:

<figure>
<img src="/blog/pictures/Snimok-ekrana-2024-02-11-v-20.13.26.png.jpg" alt="">
</figure>

Нажмите «Сохранить изменения».  
Enjoy

Спасибо за вопрос [Ольге Паньшиной](https://t.me/shrederrrrrrr)

Еще по теме  
[Как установить движок для блога Эгея](https://antonkoshuba.ru/blog/all/install-egeya/)
