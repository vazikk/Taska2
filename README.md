# Taska2
1)  Запуск instance aws 
![Image alt](https://github.com/vazikk/Taska2/blob/main/image1.png)

2)  Я сохранил приватный ключ в файле и по ssh подлкючился к серверу <br>

```ssh -i KEYTASK2.pem ec2-user@ec2-35-168-62-162.compute-1.amazonaws.com```

3)  Потом создал два юзера ```Dmitrij``` и ```jon``` <br>
![Image alt](https://github.com/vazikk/Taska2/blob/main/image2.png)

4)  Скопировал публичный ключ в ---> ```/home/Dmitrij/.ssh/authorized_keys```<br>
и установил права доступа:<br>
``` chown -R Dmitrij:Dmitrij /home/Dmitrij/.ssh```<br>
``` chmod 700 /home/Dmitrij/.ssh ```<br>
``` chmod 600 /home/Dmitrij/.ssh/authorized_keys```<br>
  
5)  После создал пароль для ```Dmitrij``` и для ```jon```<br>
  
    Проверил подлкючение на этих юзеров <br>
![Image alt](https://github.com/vazikk/Taska2/blob/main/image3.png)
__________________________________________________________________
![Image alt](https://github.com/vazikk/Taska2/blob/main/image4.png)


6)  После создал текстовый файл через ```Dmitrij``` и написал <br>
```chmod 700 hi.txt``` <br>
ограничил доступ в файлу другим пользователям и группам<br>
![Image alt](https://github.com/vazikk/Taska2/blob/main/image5.png)


7) Дал доступ к ```sudo``` ```Dmitrij``` через команду
   ``` usermod -aG wheel Dmitrij```

8) И создал еще пользователя ```Nov``` с интерпретатором bash по умолчанию
``` adduser Nov --shell /bin/bash```





