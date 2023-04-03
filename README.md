**Тестирование необходимо** для описания некоторого сценария, по которому данная функция должна работать,
и если кто-нибудь этот сценарий нарушит, изменив код, то тест об этом сообщит.
Хорошее покрытие автотестами позволяет проводить регрессионное тестирование не так часто и дает определенный гарант того,
что ваш код работает так, как было задумано.

## Пирамида тестирования - тестов нижнего слоя должно быть максимально много, а верхнего слоя максимально мало.

(Здесь от верхнего слоя к нижнему)
1. E2E - ключевая функциональность (авторизация, оплата, удаление пользователя) - 10% от общего количества;
2. INTEGRATION - несколько реакт компонентов в связке или несколько пересекающихся классов - 20-30% от общего кол-ва;
3. Скриншотные тесты - интерфейс страницы. - 70-80% вместе с unit тестами.
4. UNIT - пишутся на отдельные независимые кусочки системы (хелперы, функции, методы класса).

Изучаемые библиотеки и фреймворки:
1. Jest
2. React-testing-library (react-router-dom + redux)
3. WebdriverIO (Cypress, puppeteer, hermione)
4. Storybook + loki (скриншот-тестирование)

Виды тестирование:
1. Функциональное: модульное (unit), интеграционное, end-to-end (e2e). 
Все, что тестирует функциональность.
2. НефункциональноеЖ нагрузочное тестирование, тестирование безопасности, регрессионное тестирование.
Как система держит нагрузку, безопасность и так далее.