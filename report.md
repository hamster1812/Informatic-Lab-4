# Отчёт по лабораторной работе №4

Создадим Dockerfile для образа контейнеров
![img](scrinshots/dockerfile.png)

Построим образ
```bash
$ docker build -t image1 .
```

Запускаем контейнер при помощи команды:
```bash
$ docker run --rm --name con1 image1
```
Результат:
![img](scrinshots/fire.png)

Запустим 2ой контейнер
```bash
$ docker run --rm --name con2 image1
```

Проверим, что они работают
![img](scrinshots/cons_information.png)

Создадим сеть
![img](scrinshots/network_creating.png)

Подключим контейнеры
![img](scrinshots/connecting_cons_to_net.png)

Проверим подключение con1 к con2
![img](scrinshots/connect_con1_to_con2.png)

Проверим подключение con2 con1
![img](scrinshots/connect_con2_to_con1.png)