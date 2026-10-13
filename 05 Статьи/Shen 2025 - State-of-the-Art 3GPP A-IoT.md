---
tags: [статья]
year: 2025
venue: IEEE Comm. Standards Mag.
doi: 10.1109/MCOMSTD.2025.3573815
classification: 1/2a/2b
authors_org: China Mobile Research Institute
sector: оператор связи, Китай
---

# Shen et al. – State-of-the-Art Overview of 3GPP A-IoT Radio Access (2025)

> [!abstract] О чём
> Обзор радиоинтерфейса A-IoT от людей, которые сами его проектировали: авторы – делегаты 3GPP из China Mobile. В статье представлены конкретные значения потребления, чувствительности и дальности.

> [!info] Кто авторы
> Одиннадцать авторов из **China Mobile Research Institute** (Пекин), большая часть из отдела исследований беспроводных технологий и устройств. Ведущий автор Xiaodong Shen и другие работают инженерами по стандартизации 3GPP: 5G/6G, энергосбережением и A-IoT.
>
> Прямые участники разработки стандарта. Компания при этом сама продвигает passive IoT и ведёт испытания → [[Кейс China Mobile и Huawei]].

**На что опирается:** [[TR 38.769]] и собственные вклады авторов (Tdoc) в 3GPP.

## Что из неё вынести
|     | Вывод                                           | Подробно                                                                                                                              | Источник                                                                                                                                                                                                                              |
| --- | ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | **Device 1 очень слабый и очень неточный**      | Около 1 мкВт, уход частоты генератора до 10⁵ ppm. Device 2 – сотни мкВт и до 10⁴ ppm. Под это заточен весь протокол                   | [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf#page=2&selection=21,0,21,22\|с. 2]]                                                                                                                          |
| 2   | **Накопитель даёт выигрыш по чувствительности** | Конденсатор на 1–10 мкФ позволяет Device 1 включаться при −36 дБм, Device 2 – при −45 дБм. Это главное отличие от RFID → [[Device 1]] | [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf#page=4&selection=25,0,25,44\|с. 4]]                                                                                                                          |
| 3   | **Дальность на порядок больше, чем у RFID**     | В модели авторов: Device 1 – 36 м, Device 2 – 95 м, RFID – 2,35 м. FEC добавляет больше 4 дБ                                          | [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf#page=3&selection=151,0,151,62\|рис. 2b, с. 3]], [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf#page=3&selection=93,0,94,46\|с. 3]] |
| 4   | **Частотное разделение реально ускоряет опрос** | FDMA сокращает время инвентаризации на 46–81% → [[FDMA и малый сдвиг частоты]]                                                        | [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf#page=4&selection=88,0,88,43\|с. 4]]                                                                                                                          |
| 5   | **Сон по команде экономит энергию**             | Если сеть может усыпить устройство, это даёт около 30% времени работы                                                                 | [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf#page=5&selection=51,0,51,43\|с. 5]]                                                                                                                          |

PDF: [[State_of_the_Art_Overview_of_3GPP_Ambient_IoT_Radio_Access_Aspects.pdf]]
