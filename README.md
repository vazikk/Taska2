# Taska2
1)Запуск instance aws 
![Image alt](https://github.com/vazikk/Taska2/blob/main/image1.png)

2)Я сохранил приватный ключ в файле и по ssh подлкючился к серверу <br>

```ssh -i KEYTASK2.pem ec2-user@ec2-35-168-62-162.compute-1.amazonaws.com```

Потом создал два юзера ```Dmitrij``` и ```jon``` <br>
![Image alt](https://github.com/vazikk/Taska2/blob/main/image2.png)

Скопировал публичный ключ в ```/home/Dmitrij/.ssh/authorized_keys```<br>
  
После создал пароль для ```Dmitrij``` и для ```jon```<br>
  
Проверил подлкючение на этих юзеров <br>
![Image alt](https://github.com/vazikk/Taska2/blob/main/image3.png)




