# Прогноз активности катализатора¶
Прогноз активности катализатора На одном из предприятий СИБУР действует установка полимеризации пропилена. Ее основной продукт - гомополимер пропилена. В этой задаче вы должны построить прогноз активности катализатора, который используется в процессе полимеризации. Для решения задачи вам доступны исторические данные о работе установки.
Целевой переменной в этой задаче является активность катализатора, а прогноз должен строиться на 6 часов вперед.
В работе установки в тестовый период было несколько остановов. Активность во время остановов и сразу после них предсказывать не нужно, а точный набор временных меток, для которых необходимо построить прогноз, доступен в файле activity_test_timestamps.csv.
Данные Установка полимеризации пропилена
Установка полимеризации пропилена – технологический комплекс, предназначенный для получения порошка гомополимера пропилена.
Полимеризация осуществляется в каскаде из трех изотермических реакторов идеального перемешивания непрерывного действия в растворе в среде тяжелого растворителя (нефраса). Технологическим предшественником реакторного блока является блок приготовления катализаторного комплекса с форполимеризацией (емкости D1 и D2).
Два первичных реактора (R1 и R2) работают параллельно и независимо. Реакционная среда из них в постоянном режиме перегружается в общий вторичный реактор (R3), где происходит дополимеризация.
В процессе используется катализатор, активность которого нужно прогнозировать в этой задаче.
Исторические данные о работе установки для тренировочного периода содержатся в файле activity_train.csv.zip, а для тестового - в файле activity_test.csv.zip.
Базовое решение Простой baseline доступен в ноутбуке Baseline - Polypropylene.ipynb. Он воспроизводит тривиальное решение activity_naive_baseline.csv (последнее известное значение тренировочного периода) и создает решение на основе простой нейронной сети.
