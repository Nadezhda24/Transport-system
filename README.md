Система для реорганизации и котроля городского потока гражданского и общественного транспорта
=============
Общая информация
------------------
Основные темы:
1. Карта города с дорогами 
2. Отслеживание гражданского и маршрутного транспорта 
3. Умные светофоры
4. Количество пешеходов и пользователей общественным транспортом
5. Составление маршрутов общественного транспорта и определение его манимального количества на линии
6. Система сбора данных

Серверная часть для обработки данных
Тип клиентской части - мобильное приложение, так как данная система предполагает помогать человеку перемешаться по городу, следовательно приложение должно быть карманным.

 Приложение будет иметь следующие разделы:
 
 1. Раздел с возможностью установки постоянного класса пользователя: пешеход, пользователь общественного транспорта, водитель и т. д. Однако, каждый день необходимо будет вносить корректироваки, если класс пользователя изменится. Если корректировок нет, то учитывается постоянный класс. То есть, если человек помечает, что он водитель, но сегодня он решил отказаться от собственного транспорта, то он должен отметить это в системе.
 
 2. Раздел карты города планируется сделать в нескольких режимах в зависимости от класса пользователя(пока выделены следующие):
    
    2.1 Автомобилист:
      
        2.1.1 Отображение светофоров
      
        2.1.2 Отображение загруженности дорог  
      
        2.1.3 Подбор удобного маршрута
      
    2.2 Пешеход:
  
        2.2.1 Отображение светофоров
  
    2.3 Пользователь общественного транспорта:
      
        2.3.1 Отображение маршрутов городского транспорта с возможностью выбора необходимого
       
        2.3.2 Отображение загруженности дорог
       
        2.3.3 Подбор лучшего маршрута с учетом загруженности транспорта
        
   3. Личный кабинет пользователя, который позволит запоминать/вносить постоянные маршруты, высчитывая наилучший
 
 Анализ предметной области 
---------

### 1. Карта города 

Карты – это функциональность, которая реализуется на стороне смартфона. На Android Google Maps стоят уже по умолчанию. Это нативные карты, которые идеально заточены под Android — это позволит пользователям загружать все быстрее, и затратиться меньше времени на интеграцию. C iOS Google Maps также замечательно работают. Документация для работы с картами <https://developers.google.com/maps/documentation>. 
Карта, в данном случае, явлеяется удобным способом представления собранной информации, которая прошла обработку на сервере. То есть, практически весь результат работы системы будет отбражаен на карте. 
