# AIST_Practice_3

В этой практике была построена модель сегрегации Шеллинга.

Модель представляет собой поле, состоящее из ячеек. Поле заполнено агентами двух цветов: красного и синего. 10% ячеек остаётся пустыми.

![](/screenshots/image-1.png)

Каждый агент имеет свойство быть счастливым. Для счастья каждому агенту нужно, чтобы по соседству с ним находилось по крайней мере n = 2 агента того же цвета, что и он сам. В симуляции несчастные агенты обозначаются точкой внутри клетки.

![](/screenshots/image-2.png)

Каждый такт симуляции модель выбирает произвольного несчастного агента и позволяет ему переместиться на любую свободную клетку на поле. Модель не предлагает никакой гарантии того, что на новом месте агент будет счастлив или наоборот. После переезда свойство счастья для агентов пересчитывается.

Симуляция продолжается, пока на поле присутствуют несчастные агенты. Так выглядит конец симуляции при n = 2.

![](/screenshots/image-3.png)

Теория утверждает, что если каждый агент предпочитает иметь в качестве соседей хотя бы треть агентов того же цвета, то возникнет сегрегация. Рассмотрим более высокие значения n.

n = 3. Возникают группы (колонии) агентов одного цвета

![](/screenshots/image-4.png)

n = 4. Появляется четкое разделение групп агентов разного цвета, колонии предпочитают отделяться пустым пространством

![](/screenshots/image-5.png)

n = 5 (лучшая итерация). Четко видимые колонии, разделенные пустым пространством

![](/screenshots/image-6.png)

n = 10 (в качестве соседей рассматривается квадрат 5x5).

![](/screenshots/image-7.png)

