# РАБОТА С ПЕРЕДАТЧИКАМИ НА ЧАСТОТЕ 433Мгц С ПОМОЩЬЮ RASPBERRY PI

На этих частотах работают современные шлагбаумы, электронные ворота и некоторые электронные замки. Считав значения с приемника, когда идет сигнал с пульта для открытия чего-либо, вы можете повторить этот сигнал, тем самым открыть/закрыть цель.

Для приема и передачи используются такие типы модулей:

![alt text](https://github.com/EternalB-1/rf/tree/master/img/433.jpeg)
![alt text](https://github.com/EternalB-1/rf/tree/master/img/RD-RF5-433.jpg)

Их я подключил по схеме:

![alt text](https://github.com/EternalB-1/rf/tree/master/img/Screenshot_1.png)

Для према сигнала введите:

python3 recieve.py -g 20

Для отправки сигнала:

python3 send.py -g 21 -t * -p ** ***
*-протокол
**-pulse
***-код устройства

Вся информация взята из ролика: https://www.youtube.com/watch?v=HCiEaf1HPhE&list=PLWoFhdik2f3NByc3Zgo28IlSugXEw8_cV&index=3
