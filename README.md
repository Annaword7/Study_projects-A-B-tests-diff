# Study_projects-A-B-tests-diff methods

Для того, чтобы получать верные результаты тестирования необходимо прежде всего проверить данные, с которыми мы работаем. Если данные распределны норально, нет выбросов, и группы для сравнения всего две, то Т-тест отлично подходит. Если в данных все же пристуствуют выбросы, то лучше всего их нивелирует критерий Манна-Уитни. Бутсрап, известный, как наиболее простой метод, в даннмо случае также следует применять аккуратно, поскольку он среагировал сильно на экстремально высокие значения и не дал верного результата.

Также существуют специальные методы тестирования достверности используемых критериев. Среди них - проведение А/А тестов, датасеты исторических данных компании, установка доверительных интервалов. Что касается выбросов - в данном случае их было легко и очевидно обнаружить, но чаще всего, они встречаются в более плавноп проявлении, и тогда, среди рекомендуемых мтодов обычно приводят: -логорифмирование

критерий Манна-Уитни
убрать n% из топ
Изучив проблематику, я выяснла, что такие методы довольно часто дают ошибки в результатах, поскольку на разные сегменты пользователей тесты могут влиять по разному, и применение этих критериев хоть и даст нужный уровень P-значимости, но не даст возможности посомтреть на результаты внутри групп, которые могут взаимно перетягивать результат в нужную сторону за счет большой разницы.

Если нужно избавится от выбросов, лучше всего удалить топ пользователей на предэкспериментальном периоде. Но при этом надо помнить, что в таком случае топ пользователей может ввести себя не так, как остальные, и из-за этого вы можете принять неверное решение. Поэтому стоит дополнительно валидировать это предположение на старых A/B-тестах.

# Study_projects-A-B-tests-diff methods

In order to get the correct test results, it is necessary first of all to check the data with which we work. If the data is distributed norally, there are no outliers, and there are only two groups for comparison, then the T-test is perfect. If there are still outliers in the data, then the Mann-Whitney criterion is the best way to level them. Bootstrap, known as the simplest method, should also be used carefully in this case, since it reacted strongly to extremely high values and did not give the correct result.

There are also special methods for testing the validity of the criteria used. Among them - conducting A / A tests, datasets of historical company data, setting confidence intervals. As for emissions, in this case they were easy and obvious to detect, but most often they occur in a smoother manifestation, and then, among the recommended mtodes, they usually lead: -logorithm

Mann-Whitney criterion
to remove n% from the top
Having studied the problems, I found out that such methods quite often give errors in the results, since tests can affect different segments of users in different ways, and the application of these criteria, although it will give the right level of P-significance, will not give an opportunity to look at the results within groups that can mutually drag the result in the right direction due to big difference.

If you need to get rid of outliers, it is best to remove the top users in the pre-experimental period. But at the same time, we must remember that in this case, the top users may introduce themselves differently from the rest, and because of this you may make the wrong decision. Therefore, it is worth additionally validating this assumption on old A/B tests.
