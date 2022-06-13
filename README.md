# student-project-catalog
<h1> Коллекция студенческих проектов </h1>
В каталоге представлены "хорошие" программные проекты, выполненные в ходе лабораторных работ
с использованием технологии JavaFX

## Содержание
- Функциональность
  - [Калькулятор энергопотребления](#Калькулятор)
  - [Редактор CSS-стилей](##Редактор)
  - [Редактор CSS-стилей для fxml-форм](#визуальный_редактор)
  - [Веб-сервер совместного расписания](#веб-сервер)
  - [Редактор дорожных карт](#редактор-дорожных-карт)
  - [Редактор плана сети](#editorplanenetwork)
  - [Редактор дорожных карт проекта](#редактор-дорожных-карт-проекта)
  - [Сборщик файлов](#сборщик)
  - [Моделирование пожарной сигнализации](#сигнализация)
  - [Метеостанция](#метеостанция)
  - [Модуль авторизации](#versioning)
  - [Хранилище личных достижений](#basedata)
  - [Аквариум](#аквариум)
  - [Векторный растровый редактор](#векторый-растровый-редактор)
  - [Статистический анализатор для построения блоковых графиков](#статистический-анализатор)
  - [Прототип мобильного приложения Навигатор гостя Университета](#навигатор)
- Техники
  - [Автогенерация полей](#калькулятор)
  - [Техника чтения из файла](#калькулятор)
  - [смена сцен](#редактор)
  - [стандартные диалоги](#сборщик)
  - [Случайная генерация событий](#сигнализация)
  - [Работа с email](#basedata)
  - [Вывод в таблицу](#basedata)
  - [Поставщик-потребитель](#аквариум)
- Инструменты
  - [unit-тесты](#сигнализация)
  - [Map](#метеостанция)
  - [Система сборки Gradle](#калькулятор)
  - [Система сборки Gradle](#статистический-анализатор)
  - [canvas](#векторый-растровый-редактор)
  - [метод отсеивания тупиков](#Навигатор)
- Паттерны
  - [Абстрактная фабрика](#калькулятор)
  - [Итератор](#сборщик)
  - [Цепочка обязанностей](#Сигнализация)
  - [Медиатор](#versioning)
  - [ADO](#basedata)
  - [Builder](#статистический-анализатор)
  - [DAO](#Навигатор)
  - [Singleton](#Навигатор)
- Архитектуруы
  - [Model-View-ViewModel (MVVM)](#калькулятор)
  - [MVC](#Навигатор)
  - [Событийно-управляемая архитектура](#сигнализация)  
  - [Клиент-серверная архитектура](#метеостанция)
  - [Общий пассивный репозиторий](#basedata)
  - [MVC](#векторый-растровый-редактор)
  - [MVP](#статистический-анализатор)
  - [Каналы и фильтры (с пассивными фильтрами)](#сборщик)
  - [Каналы и фильтры (с активными фильтрами)](#аквариум)
    
# [Калькулятор](https://github.com/range36rus/power_calculate.git)
 Калькулятор энергопотребления предназначен для расчета суммарного энергопотребления различных устройств. GUI позволяет вводить/изменять значения потребляемой мощности, часов работы. Для инициализации полей загружается файл настроек, содержащий значения потребляемой мощности, используемые по умолчанию. Предусмотрена возможность его изменения на основе новых данных, получаемых от пользователя.
### Используемые методы и технологии программирования
  1. Механизм связывания для автогенерации полей GUI на основе данных в текстовом файле.
  
  Binding API (механизм связывания) предоставляет некоторые интерфейсы (например, метод bind () для одностороннего связывания), которые автоматически уведомляют объекты, когда происходит изменение значения другого объекта.
  
  2. Техника чтения из файла.
  
  Потоковый ввод-вывод с использованием классов из пакета java.io.
### Паттерны  
  1.	Использование паттерна Абстрактная фабрика для вывода значений из файла как в виде текстового поля, так в виде списка.
 
Паттерн Абстрактная фабрика позволяет создавать  семейства объектов, не инстанцируя (специфицируя) классы явно, при  этом  обеспечивается логическая связанность создаваемых объектов. 
### Инструменты
  1. Использование системы сборки Gradle.


## [Редактор](https://github.com/range36rus/cssfx-style-editor.git)
  Редактор CSS-стилей предназначен для редктирования css-стилей для fxml-форм.
  Изменения внесенные в css в текстовом редакторе, оперативно отображаюся в окне пользовательского интерфейса.
### Используемые методы и технологии программирования
  1. Смена сцен 
### Паттерны 

### Инструменты
## [Визуальный_Редактор](https://github.com/katyabarkalova/EditorCSS)
  RedactorCss имеет набор инструментов для создания и редактирования css стилей для fxml-форм. RedactorCss позволяет визуализировать в реальном времени изменения стиля
### Используемые методы и технологии программирования
  1. Смена сцен 
### Паттерны 
  1. Паттерн адаптер для работы со списокм классов и свойств
### Инструменты


## [Веб-сервер](https://github.com/pavelgulyev/WebShedule)
  Веб-сервер, использование которого в сфере организации расписания позволит повысить эффективность выполнения операций типа составления совместного расписания. 
### Используемые методы и технологии программирования
  1. Фрейворк Spring boot.
  2. MVC архитектура.
### Паттерны 
  1. Паттерн DAO  для работы с Базой данных.
### Инструменты
  1. Unit-тесты.

## [Редактор дорожных карт](https://github.com/N0RA228/ProjectTimeline)
  Данный редактор предназначен для создания и редактирования дорожных карт.
  Программа позволяет пользователю строить из нодов карту задач, редактировать, выстраивать иерархию подзадач, добавлять описание задачам, менять цвет нодов. Также программа позволяет сохранять и загружать созданные проекты. 
### Используемые методы и технологии программирования
  1. MVC архитектура.
### Паттерны 
  1. Паттерн Компоновщик.
### Инструменты
  1. Unit-тесты.

## [EditorPlaneNetwork](https://github.com/konyakovaangelina/EditorPlaneNetwork)
  Программный продукт предназначен для построения и отображения плана сети.
### Используемые методы и технологии программирования
   1. MVC архитектура.  
### Паттерны 
  1. Паттерн адаптер.
### Инструменты
  1. Unit-тесты.
  2. 
## [Редактор дорожных карт проекта](https://github.com/MaksimPodtynnikov/Offline_RoadmapBuilder)
  Программа имеет набор инструментов для создания и редактирования дорожных карт, визуализирующих шаги в работе над различными проектами. Программа позволяет контролировать выполнение задач на каждом этапе проекта. 
### Используемые методы и технологии программирования
  1. Многоуровневая структура.
  2. Событийно-ориентированная архитектура.
### Паттерны 
  1. Паттерн Адаптер.
  2. Паттерн Хранитель.
### Инструменты
  1. Unit-тесты.
  
## [Сборщик](https://github.com/vladder2312/JavaCollector.git)
 Сборщик файлов предназначен для создания листинга программного проекта.
Программный продукт позволяет собирать .java файлы в один файл внутри папки. После запуска программного продукта, необходимо выбрать директорию,в которой хранятся файлы с расширением .java. Список необходимых файлов выводится в listView. Далее, выбирается директория, куда будет записан новый файл. После, сообщение о ходе выполнения, в случае успешной или не успешной сборки. Созданный файл имеет название new.java и включает в себя все файлы из выбранной директории.
### Используемые методы и технологии программирования
  1. Использование стандартных диалогов.
### Паттерны 
  1. Паттерн Итератор для прохода по каталогу.
### Инструменты


## [Сигнализация](https://github.com/vladder2312/AlarmSystem.git)
 Система пожарной сигнализации предназначена для моделирования работы системы пожарной сигнализации. Используется событийное управление.
Датчики активируются в случайное время (шанс 30% каждую секунду). Данное событие обрабатывается следующим образом: В модель записывается номер активированного датчика и переключается цвет датчика на красный. Выводится сообщение о количестве активированных датчиках.
### Используемые методы и технологии программирования
  1. Случайная генерация событий по таймеру.
  2. Событийно-управляемая архитектура.
### Паттерны 
  1. Паттерн Цепочка обязанностей для обработки различных событий.
### Инструменты
  1. Unit-тесты.
  
  
## [Метеостанция](https://github.com/RinaKoner128/ClientServer.git)
  Сервер метеонаблюдения предназначен для сбора данных о температуре воздуха в разных населенных пунктах.
  Клиенты передают значения температуры в своем населенном пункте Серверу, могут запросить с Сервера температуру по названию города.
### Используемые методы и технологии программирования
  1. Клиент-серверная архитекутра с простым протоколом.
### Паттерны 

### Инструменты
  1. Использование Map для хранения неповторяющихся данных на Сервере.


## [basedata](https://github.com/AndreevaKristina99/DataBase.git)
  Хранилище личных достижений предназначено для хранения личных достижений в виде описания и изображения.
  Программный продукт представляет централизованное место хранения личных достижений студента с внешней базой данных. База данных хранит информацию о названии мероприятия, кратком описании, дате проведения и файле награждения. В базу данных можно добавлять и удалять личные достижения. При добавлении достижения пользователю предоставляется возможность выбора файла, с помощью диалогового окна. Информация из базы данных выводятся в элемент TableView. Программный продукт предоставляет возможность поиска по личным достижениям. Имеется возможность отправки файла из приложения на почту. Пользователь выбирает файл с помощью диалогового окна файл и отправляет его на указанный адрес.
### Используемые методы и технологии программирования
  1. Работа с email.
  2. Вывод в таблицу.
### Паттерны 
  1. Паттерн ADO.
### Инструменты


## [Аквариум](https://github.com/SashaSunsh1ne/ThreadsAquarium)
  Многопточное приложение, моделирующее аквариум с рыбками (потребителями) и кормом (поставщиками)
### Используемые методы и технологии программирования
  1. Обработка в потоках
  2. Синхронизация общего ресурса - аквариума (канвы для рисования)
### Паттерны 
  1. Поставщик-потребитель
### Инструменты
  

## [Векторый растровый редактор](https://github.com/Lyana2021/GrafRedactor)
  Графический редактор позволяет создавать, просматривать, обрабатывать и редактировать цифровые изображения (рисунки, картинки, фотографии) на компьютере.  
Предполагается работа с отдельными точками изображения, которые могут строится в виде набора: «карандаш» - соединение двух точек прямой линией шириной в 1 пиксель; «пипетка» - выбор текущего цвета; «ластик».
### Используемые методы и технологии программирования
  1. MVC архитектура.
### Паттерны 

### Инструменты
  1. Панель для рисования (canvas на fxml-форме).
  2. Пипетка(ColorPicker на fxml-форме).
  3. Ползунок для выбора толщины линии( Slider на  fxml-форме).


## [Статистический анализатор](https://github.com/range36rus/blocks-diagram)
  Статистический анализатор для построения блоковых графиков имеет возможность сохранения в файл и загрузки из него. Файл текстовый. Добавлять столбцы и строки можно бесконечно. Взаимодействовать можно с главным меню и с таблицей, а именно с её контекстным меню. 
### Используемые методы и технологии программирования
  1. Архитектура MVP
### Паттерны 
  1. Builder (для создания диаграммы)
### Инструменты
  1. Использование системы сборки Gradle.

## [Навигатор](https://github.com/dproshkeen/UniversityNavigation.git)
  Для построения маршрута сначала необходимо ввести начальную точку в поле «От». При введении названия точки, в табличной части будут появляться возможные варианты точек, по введенным данным. Необходимо выбрать из таблицы нужную начальную точку. Таким же образом заполняется поле «До»- конечная точка.
После заполнения данных о точках, необходимо нажать на кнопку «Построить» программа проложит маршрут от и до указанных точек.
В зависимости от указанных точек программа выдаст ту карту где сейчас находится пользователь и оставит доступными для переключения только те этажи, через которые будет проложен путь пользователя. Карту можно приблизить и детально рассмотреть проложенный маршрут, для этого необходимо навести на карту и покрутить колесико мышки. Если пользователь совершил ошибку при заполнении полей формы или необходимо построить новый маршрут необходимо нажать на кнопку «Сбросить». При нажатии на эту кнопку произойдет очищение всех полей формы.
### Используемые методы и технологии программирования
  1. MVC (модель, представление, контроллер)
### Паттерны
  1. DAO
  2. Singleton
### Инструменты
  1. Cоздан метод отсеивания тупиков.
