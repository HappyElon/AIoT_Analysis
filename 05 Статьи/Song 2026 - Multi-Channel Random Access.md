---
tags: [статья]
year: 2026
venue: IEEE JSAC
doi: 10.1109/JSAC.2025.3643814
classification: Type 1/2b/C
authors_org: Hanyang University
sector: университет, Южная Корея
---

# Song et al. – Dynamic Multi-Channel RA for 6G A-IoT (JSAC 2026)

> [!abstract] О чём
> Узкая исследовательская статья про одну задачу: как быстрее опросить сотни меток, если они отвечают одновременно. Авторы берут процедуру случайного доступа 3GPP, раскладывают её на несколько частотных каналов и добавляют умную подстройку длины кадра под число устройств.

> [!info] Кто авторы
> Четыре исследователя с факультета электротехники и электроники **Hanyang University** (Ансан, Южная Корея): Shilun Song, Huan Zhang, Huiyang Xie, Hu Jin. Работа поддержана программой Brain Pool Национального исследовательского фонда Кореи.
>


**На что опирается:** 3-шаговый случайный доступ A-IoT из 3GPP. Msg1 – 16-битный случайный номер, Msg2 – его эхо от сети, Msg3 – идентификатор устройства, до 8 каналов ([[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=2&selection=25,0,25,62|с. 2]], [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=4&selection=188,0,188,58|с. 4]]) → [[Протоколы случайного доступа]].

## Что из неё вынести
| | Вывод | Подробно | Источник |
|---|---|---|---|
| 1 | **Несколько каналов плюс адаптация заметно ускоряют опрос** | Авторская схема MRMC-RAP при 6 каналах и 400 устройствах на 54% эффективнее базовой процедуры; упрощённая E-RAP даёт +40% | [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=9&selection=816,0,816,57\|с. 9]], [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=5&selection=151,0,155,5\|с. 5]] |
| 2 | **Простое правило для длины кадра** | Число слотов ≈ число устройств / число каналов. С эффектом захвата правило чуть поправляется | [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=9&selection=676,0,680,7\|с. 9]], [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=10&selection=76,0,76,50\|с. 10]] |
| 3 | **Больше каналов – не всегда лучше** | Максимум эффективности приходится примерно на 4 канала | [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=10&selection=25,0,25,51\|с. 10]] |
| 4 | **Число устройств надо оценивать на лету** | Оценщик BEst считает по числу коллизий. Улучшенный BE²FT ещё и досрочно обрывает неудачный кадр | [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=11&selection=467,0,474,4\|с. 11]], [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf#page=12&selection=233,0,233,21\|с. 12]] |

PDF: [[Dynamic_Multi_Channel_Random_Access_Procedure_for_6G_Enabled_Ambient.pdf]]
