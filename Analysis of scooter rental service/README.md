Нам передали данные сервиса аренды самокатов GoFast — информацию о пользователях из нескольких городов, их поездках, ниличии подписки. Необходимо проанализировать полученные данные и проверить гипотезы, которые могут помочь бизнесу вырасти. Нужно проанализировать данные о пользователях с подпиской и без, и выяснить, действительно ли пользователи с платной подпиской приносят бизнесу более высокую прибыль.

Для анализа у нас есть три набора данных: о пользователях, их поездках и подписках.

**Описание данных**

В основных данных есть информация о пользователях, их поездках и подписках.

**Пользователи — users_go.csv**

*user_id*	- уникальный идентификатор пользователя  
*name*	- имя пользователя  
*age*	- возраст  
*city*	- город  
*subscription_type* -	тип подписки (free, ultra)  

**Поездки — rides_go.csv**

*user_id*	- уникальный идентификатор пользователя  
*distance*	- расстояние, которое пользователь проехал в текущей сессии (в метрах)  
*duration*	- продолжительность сессии (в минутах) — время с того момента, как пользователь нажал кнопку «Начать поездку» до момента, как он нажал кнопку «Завершить поездку»  
*date*	- дата совершения поездки  

**Подписки — subscriptions_go.csv**

*subscription_type*	- тип подписки  
*minute_price*	- стоимость одной минуты поездки по данной подписке  
*start_ride_price*	- стоимость начала поездки  
*subscription_fee*	- стоимость ежемесячного платежа  

Краткое описание полученных результатов.

Больше половины пользователей (54,4%) пользуюся сервисом без платной подписки. Платную подписку используют 45,6% пользователей. Услугами сервиса пользуются люди от 12 до 43 лет, а средний возраст пользователя составляет 25 лет. В целом можно сказать, что сервис проката самокатов более популярен у молодых людей - две трети пользователей не старше 28 лет.

В среднем пользователи за одну поездку проезжали около 3 километров (3070 метров). Продолжительность поездок находится в пределах от 1 минуты до 41 минуты. Две трети пользователей (75%) использовали самокат в пределах 22 минут, что вполне соотносится с тем, что две трети поездок находились в пределах 3776 метров. 
В целом, можно сказать то, что пользователи с платной подпиской совершили практически в 2 раза меньше поездок, чем пользователи без подписки, однако среднее время и среднее расстояние одной поездки у них больше.

Поездок без подписки было совершено почти в два раза больше, чем с подписками (11568 и 6500 соответственно). Пользователи с платной подпиской совершали более длинные и долгие поездки, чем пользователи без подписки. Также при разделении пользователей на две группы( с платной подпиской и без) помогло выяснить, что проблема коротких поо времни и расстоянию поездок характерна для группы пользователей без подписки.

Далее были проверены 3 гипотезы:
пользователи с подпиской тратят больше времени на поездки, чем пользователи без;
среднее расстояние, которое проезжают за одну поездку пользователи с подпиской не превышает 3130 метров;
помесячная выручка от пользователей с подпиской по месяцам будет выше, чем выручка от пользователей без подписки.
После проверки гипотез только в одном случае нулевая гипотеза не была отвергнута; в двух других - по результатам теста нулевая гипотеза была отвергнута в пользу альтернативной.
