# Описание проекта
Заказчик - стартап, который продаёт продукты питания. С помощью данных о сессиях пользователей мобильного приложения изучить воронку продаж. Дизайнеры захотели поменять шрифты во всём приложении, а менеджеры испугались, что пользователям будет непривычно. Договорились принять решение по результатам A/A/B-теста. Пользователей разбили на 3 группы: 2 контрольные со старыми шрифтами и одну экспериментальную — с новыми. Следует выяснить какой шрифт лучше.

## Цели проекта:
Изучить воронку продаж и проанализировать результаты A/A/B эксперимента, который проводился в компании с целью выяснить, является ли предложенный маркетологами новый шрифт более привлекательным для пользователей. 

## Ход исследования:
- загрузить таблицу с "логами" и проверить корректность данных;
- провести исследовательский анализ данных;
- построить и проанализировать воронку продаж;
- провести анализ результатов A/A/B-теста, выбрать статистический критерий;
- сделать выводы по результатам анализа.

## Основные выводы:
1. Анализ воронки продаж показал, что основная потеря пользователей происходит на этапе переход с Основной страницы (MainScreenAppear) на страницу выбора товаров (OffersScreenAppear). Процент людей, проходящих путь от главной страницы до оплаты составляет порядка 48%.
По итогу анализ проведенного A/A/B эксперемента можно сделать следующие выводы:
2. Несмотря на незначительное отличие в объеме выборок между группами, эксперемент был проведён корректно, что подтверждается отсутствием статистически значимых различий между контрольными группами.
3. Нельзя сказать, что предложенный дизайнерами шрифт чем то лучше того, что используется в настоящий момент. Изменение шрифта не оказало на поведение пользователей значимого эффекта, что подтверждается результатами статистических тестов между контрольными и эксперементальной группами. 

## Навыки и инструменты:
A/B тестирование, Pandas, Matplotlib, SciPy, Проверка статистических гипотез, Событийная аналитика, Продуктовые метрики

## Описание исходных данных   
Каждая запись в логе — это действие пользователя, или событие.   
EventName — название события;  
DeviceIDHash — уникальный идентификатор пользователя;  
EventTimestamp — время события;  
ExpId — номер эксперимента: 246 и 247 — контрольные группы, а 248 — экспериментальная.  
