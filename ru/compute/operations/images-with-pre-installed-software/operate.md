# Работа с виртуальной машиной на базе образа

## Подключение к виртуальной машине {#connect}

Вы можете подключиться к виртуальной машине по протоколу SSH. Для подключения по протоколу SSH укажите публичный IP-адрес виртуальной машины и закрытый ключ, соответствующий открытому ключу, переданному на виртуальную машину. IP-адрес можно узнать в консоли управления в блоке **Сеть** на странице виртуальной машины.


## Логины и пароли {#logins-passwords}

Вы можете найти логины и пароли для предустановленного программного обеспечения с помощью команды:
```
sudo cat /root/default_passwords.txt
```

Если в предустановленном программном обеспечении нет аутентификации по паролю, на виртуальной машине не будет файла с паролями.


## Использование SSL {#ssl}

Чтобы использовать SSL, самостоятельно сгенерируйте SSL-сертификат и настройте веб-сервер для работы с ним.


## Фильтрация сетевого трафика {#network-filter}

На виртуальных машинах, созданных из образов, открыты только порты, необходимые для настройки и работы предустановленного программного обеспечения. Список открытых портов для конкретной виртуальной машине вы можете посмотреть при подключении по SSH.

Чтобы открыть дополнительные порты, воспользуйтесь утилитой `iptables`.


## Установка обновлений {#updates}

Операционная система и программное обеспечение на виртуальных машинах, созданных из образов, не обновляются автоматически. Вы можете обновлять их самостоятельно.
