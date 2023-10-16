# Контейнеризация. Семинар 4.

### Задание: необходимо создать Dockerfile, основанный на любом образе (вы в праве выбрать самостоятельно).
В него необходимо поместить приложение, написанное на любом известном вам языке программирования (Python, Java, C, С#, C++).
При запуске контейнера должно запускаться самостоятельно написанное приложение.

![Снимок экрана 2023-10-17 003549](https://github.com/TellEmNo/containeriztion/assets/108148686/7c5aad63-65d7-4033-ac96-5878efe3f3d0)
![Снимок экрана 2023-10-17 003918](https://github.com/TellEmNo/containeriztion/assets/108148686/cc6a32c3-f7ad-4ba8-9edb-4b1167a61030)
![Снимок экрана 2023-10-17 004254](https://github.com/TellEmNo/containeriztion/assets/108148686/d612cd30-6f8a-4d5d-8652-c65bc0677de3)
![Снимок экрана 2023-10-17 004602](https://github.com/TellEmNo/containeriztion/assets/108148686/38449e9e-bd96-4c6a-85c2-5c2cb7bac6d8)
![Снимок экрана 2023-10-17 004611](https://github.com/TellEmNo/containeriztion/assets/108148686/f6d63090-7cad-4115-80a2-fb5a4f63ddff)
![Снимок экрана 2023-10-17 004718](https://github.com/TellEmNo/containeriztion/assets/108148686/d53c97d9-ae3c-4374-92bd-14989c3741ea)
![Снимок экрана 2023-10-17 005710](https://github.com/TellEmNo/containeriztion/assets/108148686/2e8b1865-653f-4b91-8b7c-1a77eadae5b6)
![Снимок экрана 2023-10-17 005950](https://github.com/TellEmNo/containeriztion/assets/108148686/e993c557-7d34-4019-bb7a-267d0841133b)
![Снимок экрана 2023-10-17 010033](https://github.com/TellEmNo/containeriztion/assets/108148686/8fae2c03-55aa-4331-99ff-c73b5e162f6a)
![Снимок экрана 2023-10-17 010359](https://github.com/TellEmNo/containeriztion/assets/108148686/bc78296f-9aa1-434e-92e6-ec29654f890d)

#### История команд:
1. sudo mkdir /testdocker
2. ls /
3. cd /testdocker
4. sudo nano Dockerfile
5. sudo docker build -t dockertest .
6. sudo docker run -it dockertest
7. ls
8. apt update
9. apt install nano
10. nano Dockerfile
11. exit
12. sudo nano hello.py
13. sudo nano Dockerfile
14. ls
15. sudo docker build -t dockertest .
16. sudo docker run -h Vladocker --name pythoncon dockertest
