Лабораторная работа №8.5. протокол HTTP

# Практическое задание
## Задача 1.

Адреса URL могут выглядеть очень коротко и просто, как https://ya.ru/white.  

А могут длиннее и сложнее: когда мы искали в Яндексе информацию по запросу «что такое backend», то результаты поиска получили по адресу: 

```
https://yandex.ru/search/?text=что%20такое%20backend&lr=213
```
+ В начале указывается протокол. Обычно это HTTP или HTTPS — расширение протокола HTTP.
+ yandex.ru — имя сервера.
+ `/search/` — идентификатор запрашиваемого ресурса на сервере. В этом примере мы обращаемся к сервису поиска.
+ После вопросительного знака могут идти параметры, они отделяются друг от друга символом &. В нашем случае серверу поиска были переданы два параметра:
   + `t`, со значением `что%20такое%20backend`;
   + `lr`, со значением `213`.  
      Что значит lr, пользователю неважно — имена технических параметров в каждом поисковом сервисе свои.  
 
## Задача 2.

Почувствуйте себя веб-сервером Яндекса. Вы получили страшный URL — и чтобы ответить на запрос, вам нужно сперва понять, о чём же вас спрашивают.
Расшифруйте, какой вопрос задал Яндексу пользователь.  

```
import urllib.parse


url = 'https://yandex.ru/search/?text=%D0%BA%D0%B0%D0%BA%20%D0%B1%D0%B5%D1%81%D0%BF%D0%BB%D0%B0%D1%82%D0%BD%D0%BE%20%D0%B5%D0%B7%D0%B4%D0%B8%D1%82%D1%8C%20%D0%BD%D0%B0%20%D1%82%D0%B0%D0%BA%D1%81%D0%B8'

# чтобы вычленить текст вопроса
# разбейте строку по знаку = и возьмите
# второй элемент получившегося списка 
question =  # сохраните его в переменной question

# напечатайте на экран запрос в расшифрованном виде
print(urllib.  # ваш код здесь
```

## Задание №1.

Откройте страницу курса «Python-разработчик» или «Python-разработчик Плюс» на Яндекс Практикум и в исходном коде этой страницы найдите «пасхалку», спрятанную в HTML-комментарии. Когда отыщете, переходите к следующему уроку.  

Поиск по коду станет проще, если открыть поисковую строку браузера: Ctrl + F в Windows или Cmd + F в MacOS.  

## Задача 3.

Попробуйте открыть несуществующую страницу, например вот эту, и посмотрите на код ответа. Когда откроете инструменты разработчика, не забудьте обновить страницу, чтобы увидеть HTTP-ответ. Когда найдете код ответа, переходите к следующему уроку. Если не найдёте — всё равно переходите, там интересно.  
```
Перейдите в инструменты разработчика → Network → Headers → Status Code
Обнови страницу.
```
## Задача 4.

Посмотрите через инструменты разработчика китайский поисковик baidu.com и американский yahoo.com. Найдите язык, на котором ваш браузер предпочитает видеть эти два сайта.  

```
Инструменты разработчика → Network → Doc → Headers → Request Headers → accept-language
```












 
 
