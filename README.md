# SoftArtelTest

В коде рассматриваются два варианта событий:
1.	Аргумент position совпадает с индексом “\n” в строке.
В этом случае функция возвращает 2 диапазона, общей границей которых является данный “\n”. При этом, если за/перед “\n” следует еще один “\n”, то функция возвращает “Пустой диапазон справа”, “Пустой диапазон слева”, соответственно.
Также учтен случай, когда входная строка является пустой(то есть равна “\n”), результатом работы функции будет “Пустой диапазон”.

2.	Аргумент position НЕ совпадает с индексом “\n”.
В этом случае функция возвращает один диапазон, которому принадлежит элемент с индексом position.
Если строка состоит из одного символа (не равного “\n”), то функция вернет результат в виде “[start;end]”, где и start, и end будут соответствовать этому символу.
