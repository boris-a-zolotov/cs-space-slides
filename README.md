# cs-space-slides

> Шаблон презентации для выступлений в *Computer Science Space,*
> Санкт-Петербург, 2025

## Подключенные пакеты по умолчанию

Шаблон представляет из себя документ класса `beamer` с темой по умолчанию,
в который внесены минимальные косметические изменения, чтобы он
соответствовал фирменному стилю *Computer Science Space.*

Потому пользователь может делать презентации с использованием этого шаблона,
используя привычные именно ему фичи, как будто он работает с презентацией
с нуля.

Несколько пакетов в шаблоне уже подключены заранее, это:
`[russian]{babel}`, `amssymb`, `amsmath`, `amsthm`,
`tikz` (без конкретных библиотек), `listings`.


## Название презентации, авторы, стиль презентации

Название презентации вписывать в преамбулу в стандартный TeX-овский `\title`.
С авторами чуть сложнее: чтобы было *красиво* и компилировалось
без варнингов, просим делать так, как в *minimal working example:*

```TeX
\author{\texorpdfstring{
    \Author{Имя, Фамилия 1}{Должность 1}
    \Author{Имя, Фамилия 2}{Должность 2}
}{}}
```

Авторов может быть любое количество 1–3, лишь бы прямоугольник
с их именами помещался в строку.

Есть два варианта титульной страницы, «со звёздочками» и «с чернилами».
По умолчанию установлен стиль «со звёздочками», переключение осуществляется
как в *MWE:*

```TeX
\renewcommand{\titlebackground}{\inktemplate}
```


## Как пользоваться

Сделать `fork` или скачать всё содержимое этого репозитория, вместе с
картинками и шрифтами; далее редактировать файл
[mwe-slides.tex](https://github.com/boris-a-zolotov/cs-space-slides/blob/main/mwe-slides.tex) 
на своё усмотрение, за исключением нюансов с титульной страницей,
описанных выше.


## Приглашение к сотрудничеству

Если вы хотите внести изменения в этот шаблон презентации
или предложить, как его можно было бы улучшить,
пишите в телеграм: [@boris_a_z](t.me/boris_a_z).
