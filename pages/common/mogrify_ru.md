# mogrify

> Пакетная обработка изображений, в т.ч. изменение размера, обрезка, переворачивание, добавление эффектов. Заменяет исходный файл.

- Изменить размер всех jpg изображений в папке на 50% от первоначального размера:

`mogrify -resize {{50%}} {{*.jpg}}`

- Изменить размер всех изображений, имя которых начинается с DSC, на 800x600:

`mogrify -resize {{800x600}} {{DSC*}}`

- Конвертировать все png изображения в папке в jpg:

`mogrify -format {{jpg}} {{*.png}}`

- Уменьшить насыщенность для всех изображений в папке:

`mogrify -modulate {{100,50}} {{*}}`

- Увеличить в два раза яркость для всех изображений в папке:

`mogrify -modulate {{200}} {{*}}`
