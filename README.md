<p><strong>Проект</strong>: <span>Ed-Tech. Образовательный портал существующий уже 6 год, имеющий в своей продуктовой линейке вебинары, интенсивы, курсы, подписку, повышение квалификации, лид-магниты и трипвайеры.</span></p>
<p><strong>Контекст</strong>: <span>Сформировалось понимание, что дальнейший рост невозможен без работы над показателями портала. Масштабирование трафика уже не приводит к существенному росту прибыли.</span></p>
<p><strong>Задача</strong>: <span>Для внедрения в работу портала процессов экспериментов и роста показателей необходимо было провести анализ работы портала, не масштабирует ли он в конечном счете убытки. Оцифровать то, как работает портал.</span></p>
<ul>
<li><span>Провел анализ поведения пользователей до совершения первой покупки</span></li>
<li><span>Провел анализ&nbsp; того, как покупают, через сколько времени, за сколько. Выявил разницу в покупательском поведении в зависимости от стартового продукта.</span></li>
<li><span>Составил модель юнит-экономики для понимания точек приложения усилий.</span></li>
</ul>
<p><strong>Решение</strong>: Закопаться в данные Google Analytics через BigQuery, данные покупок на протяжении года. На основе этого составить реалистичную модель юнит-экономики.</p>
<p><strong>Стек</strong>: Pandas (numpy, seaborn, datetime, matplotlib, markov-model-attribution), SQL, Google Analytics, BigQuery, Excel</p>
<p><strong>Что было сделано</strong>:</p>
<p><a href="https://nbviewer.org/github/artem-ilienkov/product_analysis_ed_tech/blob/731109d80e333ddaca1bed5386d0bd705026b528/ed_tech_ga.ipynb">Анализ поведения пользователей до совершения первой покупки</a></p>
<p>1. Выгрузил и преобразовал данные из Google Analytics в BigQuery<br />2. Исследовал кол-во дней до покупки глобально по порталу и по когортам<br />3. Построил пользовательский путь до первой покупки<br />4. Сравнил поведение пользователей, которые совершили покупки и не совершили<br />5. Использовал Цепи Маркова для определения важности точек контакта</p>
<p><a href="https://nbviewer.org/github/artem-ilienkov/product_analysis_ed_tech/blob/main/ed_tech_sales.ipynb">Анализ поведения пользователей после совершения первой покупки</a></p>
<p>1. Исследовал кол-во покупок и периоды между покупками<br />2.&nbsp;Нашел среднее кол-во покупок в каждой когорте и кол-во купленных продуктов по типам<br />3. Погрузился в средний чек, &mdash; по порталу, по когортам, в зависимости от очередности покупки, разобрался в чем причина всплеском.<br />4. Исследовал конверсию, &mdash; в первую и последующие покупки глобально и с разделение на продукты. Создал функцию считающую цепочку конверсий в зависимости от интересуемой комбинации продуктов.<br />5. Провел анализ подписки, глобально и с разделение на тарифы, периоды подписки, конверсии внутри каждого тарифа<br />6. Провел когортный анализ<br />7. Сделал выводы, определили дальнейшие шаги и построил модель юнит-экономики</p>
<p><a href="https://docs.google.com/spreadsheets/d/1wn9SelDJIRS0H85UC8_lxbvhup3n5LA88nZ3PTuQYHg/edit?usp=sharing">Модель юнит-экономики</a></p>
<p></p>
