# Quarry_Service_Agent

##  Python, Postgres, Django, Docker 

Сервис создан для информирования сотрудников компании по статусам размещенных заказов. 

## Разделы:

### Авторизация пользователя:
* имя пользователя (логин)
* пароль

### Страницы пользователя:
* Профиль пользователя 
    * Фамилия
    * Имя
    * Имя пользователя (логин)
    * Пароль
    * e-mail
    * Изменить учетную запись

**База данных по пользователям**

| ID   | e-mail            | password  | name | last name | 
|------|-------------------|-----------|------|-----------|
| No.1 | example@mail.ru   | *******   | Яир  | Фельдман  |
| No.2 | example@mail.ru   | *******   | Цви  | Рапопорт  | 


* Новости 
Здесь размещаются новости по направлениям отдела в текстовом формате. Для этого заполняется файл. 

* Состояние заказов 
Показывает информацию по заказам авторизированного пользоветеля в формате ниже:

**База данных по заказам**

| Арт.     | ENG DES                       | RUS DES                  | Кол-во | Срок изгот. | ETD/ETA SPB  | Дата поступления на склад | ЗП          | Инициатор |
|----------|-------------------------------|--------------------------|--------|-------------|--------------|---------------------------|-------------|-----------|
| 442.8800 | HYDROSET CYLINDER BUSHING     | Втулка цилиндра гидросет | 1      | 24 WEEKS    | ETD 25.10.22 | ETA 12-15/11              | ТД00-000005 | Фельдман  |
| 440.9000 | ECCENTRIC BUSH, 58/62/66/70   | Втулка эксцентриковая    | 1      | 24 WEEKS    | ETD 05.09.22 | ETA 18/10                 | ТД00-000090 | Рапопорт  | 



**Сервисы:**
сайт с информацией по заказам
рассылка менеджерам информации по заказам (1 раз в нед. автоматически)






