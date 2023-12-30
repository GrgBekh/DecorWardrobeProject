# DecorWardrobeProject

Этот проект для людей, которые хотели бы подобрать дизайн своей квартиры просто и быстро,
не обращаясь за помощью к профессионалу.

В данный момент реализован функционал: 
  * Детекции и сегментации стен
  * Извлечения карты нормалей изображения.

За детекцию и сегментацию отвечает segmentation_v01.ipynb, он работает как на искусственно созданных,
так и на реальных изображениях:

### Исходник
![alt text](Assets/102_img.png)

### Сегментация
![alt text](Assets/segmented%20102.jpg)


### Сгенерированное изображение (быть может кто-то подбирает новый дизайн с нуля и скачал изображение)

![alt text](Assets/bath.png)

За извлечение карт нормалей отвечает eval.py и прочие .py файлы(библеотеки и модули):

### Исходник
![alt text](Assets/102_img.png)

### Карта нормалей

![alt text](Assets/102_pred_norm.png)


## Credit is due

Нейронная сеть по извлечению карт нормалей была позаимствована у

https://github.com/baegwangbin/surface_normal_uncertainty

@InProceedings{Bae2021,
    title   = {Estimating and Exploiting the Aleatoric Uncertainty in Surface Normal Estimation}
    author  = {Gwangbin Bae and Ignas Budvytis and Roberto Cipolla},
    booktitle = {International Conference on Computer Vision (ICCV)},
    year = {2021}                         
}

