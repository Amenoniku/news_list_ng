# **Тестовое задание**

### Мои комментарии
За основу я взял свой "Стартовый набор" для выполнение задания. Тут у еня неплохо настроенный мной gulp. Я использую препроцессоры Jade(HTML) Stylus(CSS) и CoffeeScript(JS) но я также спокойно могу использовать любой препроцессор или писать все в чистом виде если это будет вам необходимо.

Для выполнение Задание #2 я использовал SVG и библиотечку SnapSVG так как считаю это более наглядным примером нежели через canvas.

И еще хочу добавить что верстать мне очень не по нраву, меня больше вдохновляют задачи как "Задание #2"

Вся карта проекта расположенна внизу.

## Старт проекта

##### Установка `NodeJS`

- Перейти по [ссылке](https://nodejs.org/), скачать последнюю версию и установить

##### Установка `GulpJS` глобально:
```
npm i -g gulp
```
##### Установка зависимости:
```
 npm i
```
##### Запуск Проекта:
```
 npm start
```
##### Запуск `Gulp.js`:
```
 gulp
```
* Открыть в браузере [http://localhost:8000/](http://localhost:8000/).

## Команды для запуска с Gulp.js

##### Запуск Gulp с отслеживанием изменений:
```
 gulp
```
##### Сборка брать клиентскую часть (без вотчера):
```
 gulp build
```
##### Локальный сервер на другом порте:
```
 gulp --port=Другой порт
```
##### Открыть ссылку в браузерe:
```
 gulp --open
```
##### Собрать архив всего проекта:
```
 gulp zip
```
## Структура папок и файлов
```
/                               # Корневая папка
├── content/                    # Клиентская часть 
│   ├── images/                 # Графика
│   │   ├── icons/              # SVG иконки для генерации векторного спрайта
│   │   └── sprite/             # PNG иконки для генерации растрового спрайта
│   ├── resources/              # Статические файлы
│   ├── scripts/                # Скрипты
│   │   └── app.js              # Главный скрипт
│   ├── styles/                 # Стили
│   │    ├── base/              # Базовые стили
│   │    │   ├── base.styl      # Базовый стилевой файл
│   │    │   ├── fonts.styl     # Подключение шрифтов
│   │    │   └── optimize.styl  # Сброс стилей и фиксы
│   │    ├── helpers/           # Помощники
│   │    │   ├── mixins.styl    # Примеси
│   │    │   ├── sprite.styl    # Переменные с данными PNG спрайта (автогенерация)
│   │    │   ├── svg.styl       # Переменные с данными SVG иконок (автогенерация)
│   │    │   └── variables.styl # Переменные
│   │    └── app.styl           # Главный стилевой файл
│   └── views/                  # Разметка
│          ├── layout           # Стандартная разметка
│          ├── ng-views         # Angular шаблоны
│          └── root             # Корень раазметки
├── dist/                       # Собранный проект
├── gulp/                       # Подключаемые скрипты для gulpfile.coffee
│   ├── tasks/                  # Скрипты с задачами для Gulp.js
│   ├── utils/                  # Утилиты в помощь к задачам
│   └── paths.coffee            # Список путей для генерации файлов
├── .gitignore                  # Список исключённых файлов из Git
├── gulpfile.coffee             # Файл для запуска Gulp.js
├── package.json                # Список модулей и прочей информации
└── README.md                   # Документация
```
