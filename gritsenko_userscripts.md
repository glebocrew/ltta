# Гриценко Глеб - "LTTA (Lyceum Table Tennis Application)"
### Группа: 10 - И - 3
### Электронная почта (email): glebocrew@yandex.ru
### Telegram: @glebocrew

## Пользовательские сценарии

### [ Сценарий 1 - Регистрация пользователя / Изменение профиля ]
1. Пользователь открывает приложение и нажимает кнопку регистрация.
2. Вводи Имя, Фамилию, Email (эл. почту), направление и параллель обучения и пароль два раза.
3. Система проверяет наличие почты в уже зарегистрированных.
    - Если такая почта уже есть, то система предлагает пользователю ввести другую почту. Пользователь вводит новый адрес электронной почты и повторяет шаг 3.
4. Система проверяет пароли на совпадение.
    - Если пароли не совпадают, пользователю будет предложенно ввести пароли ещё раз.
5. Система проверяет Имя и Фамилию на наличие в базе данных. Если они совпадают, то пользователю предлагается ввести другие данные.
6. Если все введённые данные корректны, пользователю отправляется письмо с кодом для подтверждения. Пользователь должен подтвердить, что почта его.
7. После успешной регистрации аккаунта, пользователя редиректит на страницу авторизации, где он сможет воспользоваться своей новой учётной записью.
8. После успешного входа в аккаунт, пользователь попадает на главную страницу.

1. Пользователь переходит в раздел "Личный кабинет".
2. Пользователь изменяет свои данные *(Фамилия, Имя, Контактная информация)*.
3. Пользователь подтверждает то, что он изменяет свою контактную информацию, вводя своё Имя, Фамилию. 
4. Пользователь меняет своё фото профиля, загруженное из галереи.

### [ Сценарий 2 - Участие в соревновании ]
1. Пользователь открывает приложение и авторизуется/регистрируется.
2. Пользователь переходит в раздел "События".
3. Пользователь выбирает нужное событие и нажимает на кнопку "Я приду!"
4. Пользователь подтверждает своё участие, вводя своё ФИ в предложенное окно (как на GitHub при удалении репозитория).
5. Во вкладке "Личный кабинет" в календаре появляется новое событие и его описание.

### [ Сценарий 3 - Просмотр турнира ]
1. Пользователь открывает приложение и авторизуется/регистрируется.
2. Пользователь переходит в раздел "События".
3. Пользователь выбирает текущее (лайв) событие, за которым он хочет следить.
4. У пользователя появляется лайв таблица турнирной сетки, таблица сетов(партий/встреч) список участников и их текущих дельт.

### [ Сценарий 5 - Просмотр своего рейтига ]
1. Прользователь переходит в раздел "Личный кабинет" и видит свой рейтинг.
2. Если пользователь хочет найти себя в таблице всех зарегистрированных лицеистов, ему требуется сделать следующие шаги.
3. Пользователь переходит в раздел "Рейтинг".
4. Пользователь находит себя в поисковой строке или при помощи скролла.
5. Пользователь смотрит свой рейтинг.

### [ Сценарий 6 - Поиск игрока в рейтинге ]
1. Пользователь переходит в раздел "Рейтинг".
2. Пользователь выбирает фильтр по группе/по зданию/по параллели.
3. Пользователь находит либо себя либо сравнение рейтинга и своё место в лидерборде.

### [ Сценарий 7 - Скачивание хроник соревнований с выделением своего пути ]
1. Пользователь переходит в завершившееся соревнование.
2. Пользователь нажимает на кнопку "Скачать Соревнование"
3. У пользователя сохраняется хроника соревнование, как файл, где его ФИО в каждом этапе выделено.

### [ Сценарий 8 - Скачивание профиля ]
1. Пользователь переходет в раздел "Рейтинг".
2. Пользователь переходит в интересующий его профиль.
3. Пользователь нажимает на кнопку "Скачать Профиль".
4. На пользовательском устройстве сохраняется статистика о пользователе.

### [ Сценарий 9 - Календарь событий ]
1. Пользователь входит в раздел "Личный кабинет".
2. Пользователь переходит к календарю событий.
3. Пользователь находит интересующее событие и нажимает на него.
4. Пользователь просматривает содержимое.

### [ Сценарий 10 - Помощь ]
1. Пользователь входит в раздел "Помощь".
2. Пользователь переходит к интересующему пункту.
3. Пользователь читает мануал.

## Администраторские сценарии
### [ Сценарий 11 - Добавление/удаление нового администратора/редактора ]
1. Администратор переходит в специальный раздел "Участники".
2. Администратор выбирает участника и нажимает на кнопку "Изменить права".
3. Администратор выбирает с какими правами будет участник:
    - Администратор - полный доступ ко всем действиям на сайте.
    - Редактор - полный доступ ко всем действиям на сайте, за исключением добавления новых администраторов.
4. Администратор нажимает на кнопку "Сохранить изменения".
5. В случае исключения администратора по каким-либо причинам, администратор нажимает также на кнопку "Изменить права" и подтверждает своё действие.

### [ Сценарий 12 - Создание соревнования/события ]
1. Администратор переходит в раздел "События".
2. Администратор нажимает на кнопку "Создать событие".
3. Администратор выбирает тип события "Соревнование".
4. Администратор изменяет *время события, фото события, описание события и заголовок события*. 
5. Администратор выбирает кликами и с помощью строки поиска участников соревнования.
6. Администратор подтверждает, что он ввёл событие правильно и нажимает на кнопку "Опубликовать соревнование"

### [ Сценарий 13 - Изменение события/события ]
1. Администратор переходит в раздел "События".
2. Администратор выбирает нужное ему событие/сорвенование.
3. Администратор изменяет данные *время события, фото события, описание события и заголовок события*, для соревнования доступно изменение положения игроков (вместо 0:0 вписать исход встречи и победителя).
4. Администратор нажимает на кнопку "Применить изменения".

### [ Сценарий 14 - Завершение события ]
1. Администратор переходит в раздел "События".
2. Администратор выбирает интересующее его событие.
3. Администратор нажимает завершить событие.
4. Регистрация на данное событие и/или изменение его данных невозможно.

### [ Сценарий 15 - Изменение рейтинга игрока ]
Изменение рейтинга игрока происходит: <br>
1. Автоматически при завершении соревнования.
2. При ручном изменении администратором:
    1. Администратор находит интересующего спортсмена.
    2. Администратор нажимает на кнопку "Изменить данные".
    3. Администратор изменяет рейтинг игрока.
    4. Администратор нажимает на кнопку "Сохранить изменения".

### [ Сценарий 16 - Скачивание таблицы спортсменов, зарегистрировавшихся на турнир/событие ]
1. Администратор переходит в интересующее событие.
2. Администратор нажимает на кнопку "Скачать Участников".
3. У администратора на устройстве сохраняется таблица участников события

### [ Сценарий 17 - Изменение учётной записи игрока ]
1. Администратор переходит в раздел "Участники".
2. Администратор выбирает интересующего его участника.
3. Администратор нажимает кнопку "Изменить".
4. Администратор изменяет данные.
5. Администратор нажимает кнопку "Сохранить Изменения".

### [ Сценарий 18 - Справка для администратора ]
1. Администратор переходит в раздел "Справка".
2. Администратор переходит в интересующий его пункт.
3. Администратор читает справку.