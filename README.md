# student-project-catalog
<h1> Коллекция студенческих проектов </h1>
В каталоге представлены "хорошие" программные проекты, выполненные в ходе лабораторных работ
с использованием технологии JavaFX

## Содержание
- Функциональность
  - [Калькулятор энергопотребления](#калькулятор)
  - [Редактор CSS-стилей](#редактор)
  - [Сборщик файлов](#сборщик)
  - [Моделирование пожарной сигнализации](#сигнализация)
  - [Метеостанция](#метеостанция)
  - [Модуль авторизации](#versioning)
  - [Хранилище личных достижений](#basedata)
  - [Аквариум](#аквариум)
  - [Векторный растровый редактор](#Векторный растровый редактор)
  - [Статистический анализатор для построения блоковых графиков](#Статистический анализатор)
  - [Прототип мобильного приложения Навигатор гостя Университета](#Навигатор)
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
  - [Система сборки Gradle](#Статистический анализатор)
  - [canvas](#Векторный растровый редактор)
  - [метод отсеивания тупиков](#Навигатор)
- Паттерны
  - [Абстрактная фабрика](#калькулятор)
  - [Итератор](#сборщик)
  - [Цепочка обязанностей](#Сигнализация)
  - [Медиатор](#versioning)
  - [ADO](#basedata)
  - [Builder](#Статистический анализатор)
  - [DAO](#Навигатор)
  - [Singleton](#Навигатор)
- Архитектуруы
  - [Model-View-ViewModel (MVVM)](#калькулятор)
  - [MVC](#Навигатор)
  - [Событийно-управляемая архитектура](#сигнализация)  
  - [Клиент-серверная архитектура](#метеостанция)
  - [Общий пассивный репозиторий](#basedata)
  - [MVC](#Векторный растровый редактор)
  - [MVP](#Статистический анализатор)
  - [Каналы и фильтры (с пассивными фильтрами)](#сборщик)
  - [Каналы и фильтры (с активными фильтрами)](#аквариум)
    
## [Калькулятор](https://github.com/range36rus/power_calculate.git)
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


## [versioning](https://github.com/RinaKoner128/ClientServer.git)
  Модуль авторизации предназначен для переключения режима работы в зависимости от вида пользователя.
### Используемые методы и технологии программирования
  
### Паттерны 
  1. Паттерн Медиатор
### Инструменты



## [basedata](https://github.com/AndreevaKristina99/DataBase.git)
  Хранилище личных достижений предназначено для хранения личных достижений в виде описания и изображения.
  Программный продукт представляет централизованное место хранения личных достижений студента с внешней базой данных. База данных хранит информацию о названии мероприятия, кратком описании, дате проведения и файле награждения. В базу данных можно добавлять и удалять личные достижения. При добавлении достижения пользователю предоставляется возможность выбора файла, с помощью диалогового окна. Информация из базы данных выводятся в элемент TableView. Программный продукт предоставляет возможность поиска по личным достижениям. Имеется возможность отправки файла из приложения на почту. Пользователь выбирает файл с помощью диалогового окна файл и отправляет его на указанный адрес.
### Используемые методы и технологии программирования
  1. Работа с email.
  2. Вывод в таблицу.
### Паттерны 
  1. Паттерн ADO.
### Инструменты



## [Аквариум](ссылка)
  (Описание)
### Используемые методы и технологии программирования
  1. Поставщик-потребитель.
  2. Каналы и фильтры (с активными фильтрами).
### Паттерны 

### Инструменты
  


## [Векторый растровый редактор](ссылка)
  Графический редактор позволяет создавать, просматривать, обрабатывать и редактировать цифровые изображения (рисунки, картинки, фотографии) на компьютере.  
Предполагается работа с отдельными точками изображения, которые могут строится в виде набора: «карандаш» - соединение двух точек прямой линией шириной в 1 пиксель; «пипетка» - выбор текущего цвета; «ластик».
### Используемые методы и технологии программирования
  1. MVC архитектура.
### Паттерны 

### Инструменты
  1. Панель для рисования (canvas на fxml-форме).


## [Статистический анализатор](ссылка)
  Статистический анализатор для построения блоковых графиков имеет возможность сохранения в файл и загрузки из него. Файл текстовый. Добавлять столбцы и строки можно бесконечно. Взаимодействовать можно с главным меню и с таблицей, а именно с её контекстным меню. 
### Используемые методы и технологии программирования
  1. Архитектура MVP
### Паттерны 
  1. Builder (для создания диаграммы)
### Инструменты
  1. Использование системы сборки Gradle.

## [Навигатор](ссылка)
  Для построения маршрута сначала необходимо ввести начальную точку в поле «От». При введении названия точки, в табличной части будут появляться возможные варианты точек, по введенным данным. Необходимо выбрать из таблицы нужную начальную точку. Таким же образом заполняется поле «До»- конечная точка.
После заполнения данных о точках, необходимо нажать на кнопку «Построить» программа проложит маршрут от и до указанных точек.
В зависимости от указанных точек программа выдаст ту карту где сейчас находится пользователь и оставит доступными для переключения только те этажи, через которые будет проложен путь пользователя. Карту можно приблизить и детально рассмотреть проложенный маршрут, для этого необходимо навести на карту и покрутить колесико мышки. Если пользователь совершил ошибку при заполнении полей формы или необходимо построить новый маршрут необходимо нажать на кнопку «Сбросить». При нажатии на эту кнопку произойдет очищение всех полей формы.
### Используемые методы и технологии программирования
  1. MVC (модель, представление, контроллер)
№№№ Паттерны
  1. DAO
  2. Singleton
### Инструменты
  1. Cоздан метод отсеивания тупиков.
