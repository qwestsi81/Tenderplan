# Внедрение отчетности по тендерам в компанию. 

**Цель проекта**

Автоматизация сбора информации по закупкам  из портала [tenderplan.ru](https://tenderplan.ru/) и формирование автоматизированной управленческой отчетности по закупкам в разрезе сторудников, регионов, площадок закупок.

**Задачи проекта**

- автоматизация процесса выгрузки информации из площадки по закупкам [tenderplan.ru](https://tenderplan.ru/) в БД;
- формирование представления данных на стороне БД;
- формирование дашборда на стороне PowerBI.

**Инструменты для реализации проекта**

- python (requests, beautifulsoup, pandas, numpy, коннекторы к mysql);
- SQL (реализация представлений данных на стороне СУБД MySQL);
- PowerBI (M, DAX, CG).

**Этапы проекта**

- формирование подключения к [API tenderplan](https://tenderplan.ru/api/doc/);
- парсинг информации по субъектам РФ из [Википедиа](https://ru.wikipedia.org/wiki/%D0%A1%D1%83%D0%B1%D1%8A%D0%B5%D0%BA%D1%82%D1%8B_%D0%A0%D0%BE%D1%81%D1%81%D0%B8%D0%B9%D1%81%D0%BA%D0%BE%D0%B9_%D0%A4%D0%B5%D0%B4%D0%B5%D1%80%D0%B0%D1%86%D0%B8%D0%B8);
- преобразование информации;
- создание БД и объектов в ней со всеми связями;
- настройка автоматической загрузки информации из портала в БД;
- создание view, для последующей загрузки в PowerBI;
- создание дашборда в PowerBI.

**Ссылки на тетради**

- [создание БД](https://github.com/qwestsi81/Tenderplan/blob/main/pet/create_DB.ipynb);
- [справочник субъектов РФ](https://github.com/qwestsi81/Tenderplan/blob/main/pet/dict_region.ipynb);
- [справочник меток закупок](https://github.com/qwestsi81/Tenderplan/blob/main/pet/dict_marks.ipynb);
- [справочник сотрудников компании](https://github.com/qwestsi81/Tenderplan/blob/main/pet/dict_users.ipynb);
- [справочник статусов закупок](https://github.com/qwestsi81/Tenderplan/blob/main/pet/dict_status.ipynb);
- [справочник типов закупки](https://github.com/qwestsi81/Tenderplan/blob/main/pet/dict_placingway.ipynb);
- [список тендеров для создания тб фактов и справочника тендеров](https://github.com/qwestsi81/Tenderplan/blob/main/pet/lst_%D1%82enders.ipynb);
- [таблицы фактов и справочник тендера](https://github.com/qwestsi81/Tenderplan/blob/main/pet/df_tenders.ipynb);
- [наполнение БД](https://github.com/qwestsi81/Tenderplan/blob/main/pet/alter_incert_DB.ipynb);
- [создание view](https://github.com/qwestsi81/Tenderplan/blob/main/pet/creat_view.ipynb);
- [выполнение программы](https://github.com/qwestsi81/Tenderplan/blob/main/pet/%D0%9E%D1%82%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0%20%D1%81%D0%BA%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D0%B2.ipynb).

**Ссылки на прочие файлы**

- [схема БД](https://github.com/qwestsi81/Tenderplan/blob/main/pet/%D0%A1%D1%85%D0%B5%D0%BC%D0%B0%20%D0%91%D0%94.png).
