# Начало
Работа с АВЛ деревьями C++
### Текущее задание

+ getMax()  = внутри вызывает себя для Node.right, пока не упрется в лист и выводит его key

+ getMin()  = внутри вызывает себя для Node.left, пока не упрется в лист и выводит его key

+ find(key_f)  = ищет элемент, двигаясь относительно нод (если больше - вызывается правая нода, если меньше текущей - вызывается левая)

+ printTree()  = симметричный обход: внутри метод вызывается для: 1)левого, 2) выводиться key, 3)правого. как итог должна получиться возрастающая последовательность

+ deleteTree()  = обратный обход: внутри метод вызывается для: 1) левый, 2) правый, 3) вывод key и удаление ноды

+ copyTree()  = прямой обход: внутри метод вызывается для: 1) key, 2) левый, 3) правый. так можно перенести дерево сверху вниз.

+ insert(key_n)  = вызывается поиск для key_n и если нода = Null - вставляем новую ноду с этим значением

+ delete(node_d)  = нужно сделать удаление листа, удаление ноды с одним листом, и удаление ноды с несколькими листами. последнее нужно реализовать через node_d.left.getMax() или через node_d.right.getMin(). найденная нода заменяет удаляемую, а на месте найденной ставим Null.
