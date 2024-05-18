# Домашнее задание к лекции 4 «Проведение нагрузочного тестирования DB»

Любые вопросы по решению задач задавайте в чате учебной группы.

### Задание 1

Провести тестирование процедур dorepeat_v1 и dorepeat_v2, прислать скриншоты графиков.

### Что нужно сделать

Нужно провести тестирование хранимой процедуры:
1. Измерить время отклика вызова процедуры dbrepeat_v1.
2. Измерить время отклика вызова процедуры dbrepeat_v2. Для процедуры нужно дополнительно передать текст комментария p2.

#### Отправка задания на проверку

Нужно запушить репозиторий с конфигурацией, дашбордами и скриншотами на GitHub и отправить на проверку ссылку на репозиторий.

#### Задание 2* (необязательное)

Провести тестирование Web + DB. В одном тест-плане добавить 2 потока, со своим сценарием для каждого. 

### Что нужно сделать

Проверсти веб-тестирование одного поста с одним комментарием и с одним миллионом комментариев, прислать скриншоты графиков. 
  Группа сценариев.
   
Сценарий 1:
- пользователь читает комментарии к [посту](https://qamidhl.herokuapp.com/?p=1), обновляя страницу.

Сценарий 2:  
- через БД заполнять комментариями WP 100 комментариев в 1 секунд;
- опеределить точку отказа, при каком количестве комметариев к посту у пользователя страница начинает загружаться больше 20 секунд.

#### Отправка задания на проверку

Нужно запушить репозиторий с конфигурацией, дашбордами и скриншотами на GitHub и отправить на проверку ссылку на репозиторий.

### Дополнительная информация
- [build-db-test-plan](https://jmeter.apache.org/usermanual/build-db-test-plan.html) — инструкция создания теста DB с нуля.
- [mysql-db-driver](https://dev.mysql.com/downloads/connector/j/) — драйвер с официального сайта для установка в JMeter/Lib.

<details>
  <summary>Подсказка.</summary>
  
  Используйте примеры из папки [./jmeter](./jmeter) для запуска теста, а библиотеку [mysql-connector-java-8.0.28.jar](./jmeter/mysql-connector-java-8.0.28.jar) — для подключения к MySQL, если не удалось скачать из интернета.
</details>
