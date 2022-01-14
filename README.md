# Data_project
Проект по имплементации Свёрточной нейронной сети с точностью в 91% в приложении Django, для визуального подтверждения предсказаний сети

Веб интерфейс создан на основе фреймворка Django, благодаря которому сокращается время создания самого приложения. Фреймворк позволяет создавать сайт из компонентов имея подключаемую архитектуру приложений, встроенный интерфейс администратора и много других преимуществ. Благодаря реализации функции predict: идет загрузка изображения, преобразования в массив, сжатие. Также делаем предсказание с использованием нашей загруженной нейронной сети для этого изображения.

В обычном перцептроне, который представляет собой полносвязную нейронную сеть, каждый нейрон связан со всеми нейронами предыдущего слоя, причём каждая связь имеет свой персональный весовой коэффициент. 
В свёрточной нейронной сети в операции свёртки используется лишь ограниченная матрица весов небольшого размера, которую «двигают» по всему обрабатываемому слою (в самом начале — непосредственно по входному изображению), формируя после каждого сдвига сигнал активации для нейрона следующего слоя с аналогичной позицией. То есть для различных нейронов выходного слоя используются одна и та же матрица весов, которую также называют ядром свёртки. Её интерпретируют как графическое кодирование какого-либо признака, например, наличие наклонной линии под определённым углом. Тогда следующий слой, получившийся в результате операции свёртки такой матрицей весов, показывает наличие данного признака в обрабатываемом слое и её координаты, формируя так называемую карту признаков


Используемые концепции при создании сети:

Увеличение количесвта данных(DATA AUGMENTATION) - это стратегия, которая позволяет  значительно увеличить разнообразие данных, доступных для обучающих модели, без сбора новых данных. Для обучения используются методы увеличения данных, такие как обрезка, заполнение и горизонтальное отражение.

Нормализация : Пакетная нормализация (BATCH-NORMALIZATION) - это метод повышения скорости, производительности и стабильности искусственных нейронных сетей. Он используется для нормализации входного слоя путем повторного центрирования и масштабирования изображения.


![Untitled Diagram](https://user-images.githubusercontent.com/75742778/147501813-cbc030ca-7f89-4b77-9f15-5634a3519b99.jpg)
