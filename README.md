# obrabMultimediaLab5

### Step decay
Оранжевый= ( init_lr = 0.1, drop = 0.23, epoch_drop = 8.24)
Синий= ( init_lr = 0.1, drop = 0.2, epoch_drop = 10.0)
Красный= ( init_lr = 0.1, drop = 0.8, epoch_drop = 5.0)
Голубой= WarmUp ( init_lr = 0.001, drop = 0.5)

На обучающей выборке:

1) На графике точности лучше всех сошелся Голубой с WarmUp, остальные же не сошлись. Ближе всех к тому чтобы сойтись оказался Красный ( конечное значение 0.86).

2) На графике потерь все сходятся примерно одинаково. Опять можно выделить Голубой с WarmUp у которого начальное значение меньше, чем у остальных.
![1](https://github.com/IGRICHINSKYBSU/obrabMultimediaLab5/raw/master/1.jpg) 
![1](https://github.com/IGRICHINSKYBSU/obrabMultimediaLab5/raw/master/2.jpg) 

На валидационной выборке 

1) На графике точности лучше всех себя показал Голубой, хотя не дошел до конца, остальные же графики примерно повторяют друг друга. Лучшим среди оставшихся трех является Оранжевый
так как имеет все же большую точность на верхних пиках, а нижние наименьшие среди остальных.

2) На графике потерь лучший опять Голубой, но он не дошел до конца. Среди оставшихся в самом конце наименьшее значение имеет Оранжевый 0.621, хоть в самом начале он и имел наибольший из всех выброс.
![1](https://github.com/IGRICHINSKYBSU/obrabMultimediaLab5/raw/master/3.jpg) 
![1](https://github.com/IGRICHINSKYBSU/obrabMultimediaLab5/raw/master/4.jpg) 
![1](https://github.com/IGRICHINSKYBSU/obrabMultimediaLab5/raw/master/5.jpg) 
Лучшая сходимость при обучении Голубой= WarmUp ( init_lr = 0.001, drop = 0.5)

### Exponential decay
