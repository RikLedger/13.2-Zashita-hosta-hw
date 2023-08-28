# Домашнее задание к занятию 13.2 "Защита хоста" - `Горбачев Олег`

Любые вопросы по решению задач задавайте в чате учебной группы.

### Задание 1.
Установите eCryptfs.

Добавьте пользователя cryptouser.

Зашифруйте домашний каталог пользователя с помощью eCryptfs.

В качестве ответа пришлите снимки экрана домашнего каталога пользователя с исходными и зашифрованными данными.

___
### Ответ:

Доомашний католог, создадим пользователя `cryptouser`.

**Скриншот**

![Домашний католог](https://user-images.githubusercontent.com/94833070/205437175-0658f5fa-f5e3-4188-9714-648e29d1313f.png)


Зашифруем домашний каталог /home пользователя cryptouser с помощью eCryptfs.

**Скриншот**

![шифрование](https://user-images.githubusercontent.com/94833070/205437182-e450d529-e1d3-4d6d-a201-708b95e9721e.png)


**Зашифрованный раздел /home**

**Скриншот**

![Видим зашифрованный раздел](https://user-images.githubusercontent.com/94833070/205437047-bc24c9ed-a51c-45a5-9dae-b42b999071ed.png)

Возвращяем доступ к файлам папки /home 

**Скриншот**

![Размонтирование и доступ к файлам](https://user-images.githubusercontent.com/94833070/205437191-dcd34637-63e7-450f-bb6e-c82bd99ebf1f.png)


Как видим доступ появился в домашней папке /home 

# Задание 2.
Установите поддержку LUKS.

Создайте небольшой раздел (например, 100 Мб).

Зашифруйте созданный раздел с помощью LUKS.

В качестве ответа пришлите снимки экрана с поэтапным выполнением задания.

___
**Ответ:**

Зашифруем созданный раздел sbd = 100 Мб с помощью LUKS.

**Скриншот**

![Снимок экрана от 2022-12-04 14-13-37](https://user-images.githubusercontent.com/94833070/205483850-f60543aa-c30c-4aca-b750-77e1d16a0512.png)

проверяем 

**Скриншот**

![Снимок экрана от 2022-12-04 14-16-32](https://user-images.githubusercontent.com/94833070/205483878-e0a019b6-4114-42ab-9587-ecd58d918f24.png)


Чтобы расшифровать диск, который был зашифрован с помощью LUKS. Требуется выполнить и смонтировать диск 

**Скриншот**

![Снимок экрана от 2022-12-04 14-18-19](https://user-images.githubusercontent.com/94833070/205483958-d6a9fde7-ef7e-4e0e-9a36-277a61535150.png)

точка монтирования для подключенного диска.  /media/mydrive 

проверим

**Скриншот**

![Снимок экрана от 2022-12-04 14-21-35](https://user-images.githubusercontent.com/94833070/205484139-34fead3b-d96b-40c7-b144-371725916810.png)

После подключения мы сможем получить доступ к подключенному диску из графического файлового менеджера или из командной строки.
