---
title: "Верстаем письмо в ХТМЛ"
date: 2024-01-21T12:29:27+05:00
slug: "pismo-v-html"
blogtags:
  - "технодурка"
aegea_id: 18
---

Бывают ситуации, когда надо красиво и предсказуемо сверстать письмо. Например, ответное письмо при регистрации на вебинар или отклик на вакансию или небольшая рассылка, когда не нужны платные сервисы емаил рассылок.

**В чем проблема**  
Интерфейс почтовых клиентов не позволяет тонко настроить типографику письма, задать точный кегль, интерлиньяж, отступы. Приходится мириться с тем, что есть, использовать базовые шрифты и размеры. В некоторых программах типа [Thunderbird](https://www.thunderbird.net/ru/) можно прописывать стили письма, но этого все равно недостаточно.

**Как решить**

1. Подготовить шаблон письма в ХТМЛ
2. Создать новое письмо в gmail
3. Открыть инспектор кода
4. Удалить тег < br > и вставить на его место код письма

## Готовим шаблон письма в ХТМЛ

Я взял обычный шаблон из сервиса рассылок. Вы можете сделать свой или взять этот, настроить его так, как вам хочется.

```
<table align="left" border="0" cellpadding="0" cellspacing="0" style="max-width: 100%;min-width: 100%;border-collapse: collapse;mso-table-lspace: 0pt;mso-table-rspace: 0pt;-ms-text-size-adjust: 100%;-webkit-text-size-adjust: 100%;" width="100%">
<tbody>
<tr>
<td style="padding-top: 0;padding-right: 18px;padding-bottom: 9px;padding-left: 18px;mso-line-height-rule: exactly;-ms-text-size-adjust: 100%;-webkit-text-size-adjust: 100%;word-break: break-word;color: #202020;font-family: Helvetica; line-height: 150%;text-align: left;" valign="top">

<h2 style="display: block; margin: 0; padding: 0; font-family: Helvetica;font-size: 22px;font-style: normal;font-weight: bold; line-height: 125%; letter-spacing: normal;text-align: left;">Поздравляю с успешной регистрацией на вебинар «Вебмастер 2024»</h2>

<p style="margin: 10px 0; font-size: 16px; line-height: 150%;">Вебинар пройдет в воскресенье <a href="https://calendar.google.com/calendar/event%E2%80%A6">28 января в 11:00 по Мск</a> в зуме.<br>
Я планирую уложиться в 1 час, но на всякий случай запланируйте 1,5 часа на вебинар.</p>

<p style="margin: 10px 0; font-size: 16px; line-height: 150%;">За 30 минут до начала мы отправим ссылку на вход.</p>
				</td>
			</tr>
		</tbody>
	</table>
```

## Создаем новое письмо в gmail

<figure>
<img src="/blog/pictures/1.png" alt="">
</figure>

## Открываем инспектор кода

Кликаем правой кнопкой мыши и выбираем «Посмотреть код». В [Mozilla Firefox](https://www.mozilla.org/ru/firefox/new/) этот пункт называется «Исследовать».

<figure>
<img src="/blog/pictures/2.png" alt="">
</figure>

## Редактируем код и вставляем туда наш шаблон

Когда откроется инспектор кода, в нем будет выделен участок отвечающий за содержимое письма.  
Кликаем правой клавишей по выделенному блоку и выбираем «Edit as HTML».

<figure>
<img src="/blog/pictures/3.png" alt="">
</figure>

Удаляем тег < br > и вставляем вместо него ХТМЛ-код письма.

<figure>
<img src="/blog/pictures/4.png" alt="">
<img src="/blog/pictures/5.png" alt="">
</figure>

<figure>
<img src="/blog/pictures/5.png" alt="">
</figure>

После этого останется только добавить получателей и тему письма.
