# Контейнеризация. Семинар 3.

### 1 - Устанавливаем Докер

![Снимок экрана 2023-10-13 010455](https://github.com/TellEmNo/containeriztion/assets/108148686/045238fa-e398-40a7-87ba-d5b1e17e64de)
![Снимок экрана 2023-10-13 010525](https://github.com/TellEmNo/containeriztion/assets/108148686/1ff40000-981d-46bf-843d-86a5a9609e94)
![Снимок экрана 2023-10-13 010648](https://github.com/TellEmNo/containeriztion/assets/108148686/b91fff1d-44c5-481a-b18d-86230c191b32)
![Снимок экрана 2023-10-13 010909](https://github.com/TellEmNo/containeriztion/assets/108148686/bf8a7d5f-6a1d-4d0e-b1dc-4b89454a694e)
![Снимок экрана 2023-10-13 011028](https://github.com/TellEmNo/containeriztion/assets/108148686/65247d38-cc42-44a8-8a97-c3ffacfb0684)
![Снимок экрана 2023-10-13 011302](https://github.com/TellEmNo/containeriztion/assets/108148686/0d8833d9-00ff-4362-b146-ea4482f3589c)

##### История команд:

1. sudo apt update
2. sudo apt upgrade
3. sudo apt install apt-transport-https ca-certificates curl software-properties-common
4. curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
5. echo "deb [signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
6. sudo apt update
7. sudo apt install docker-ce
8. sudo usermod -aG docker $USER
9. newgrp docker
10. docker --version
___

### 2 - Тестируем.

![Снимок экрана 2023-10-13 013625](https://github.com/TellEmNo/containeriztion/assets/108148686/aa930bca-9f89-435b-927e-f3e262474b94)
![Снимок экрана 2023-10-13 013644](https://github.com/TellEmNo/containeriztion/assets/108148686/b257e529-cc05-4dfd-a034-f2c5dbeaac61)
![Снимок экрана 2023-10-13 014459](https://github.com/TellEmNo/containeriztion/assets/108148686/a85814f4-1c5b-4ff9-a00f-f5cbbccc2bec)
![Снимок экрана 2023-10-13 014509](https://github.com/TellEmNo/containeriztion/assets/108148686/b3ecd22c-e01e-42f4-b431-e2edb2bcb512)

##### История команд:

1. docker run docker/whalesay cowsay Hello, Docker!
2. docker run docker/whalesay cowsay -f elephant "Hello, Docker!"
3. docker run docker/whalesay cowsay -f tux "Hello, Docker!"
4. docker run docker/whalesay cowsay -f dragon "Hello, Docker!"
5. docker run docker/whalesay cowsay -f kangaroo "Hello, Docker!"
6. docker run docker/whalesay cowsay -f duck "Hello, Docker!"
7. docker run docker/whalesay cowsay -f panda "Hello, Docker!"
8. docker run docker/whalesay cowsay -f owl "Hello, Docker!"
9. docker run docker/whalesay cowsay -f kitty "Hello, Docker!"
___

### 3 - Тестируем команды.

![Снимок экрана 2023-10-13 015725](https://github.com/TellEmNo/containeriztion/assets/108148686/4d3e465c-1fa7-40b3-bad2-283bdf7a7241)
![Снимок экрана 2023-10-13 015737](https://github.com/TellEmNo/containeriztion/assets/108148686/f974b8be-6ba4-4065-9edb-09420cb9a9bb)
![Снимок экрана 2023-10-13 015855](https://github.com/TellEmNo/containeriztion/assets/108148686/569fbf88-ae1a-4910-af62-3691b8fe4f97)

##### История команд:

1. docker images
2. docker ps -a
3. docker rmi 6b362a9f73eb --force
4. docker rm $(docker ps -aq)  или  docker rm $(docker ps -a -q -f status=exited)
5. docker ps -a
___

### 4 - Хранение данных в контейнерах Docker: Руководство с пояснениями.

![Снимок экрана 2023-10-13 020355](https://github.com/TellEmNo/containeriztion/assets/108148686/85f16e03-04ce-432f-8aa0-f7f17e909889)
![Снимок экрана 2023-10-13 020459](https://github.com/TellEmNo/containeriztion/assets/108148686/7b88a3c5-2204-4a24-afd7-63347b4c25a8)
![Снимок экрана 2023-10-13 020637](https://github.com/TellEmNo/containeriztion/assets/108148686/98da7cde-4314-4d53-a566-9d4cd9c299b2)
![Снимок экрана 2023-10-13 021708](https://github.com/TellEmNo/containeriztion/assets/108148686/4f5d0741-70b1-4707-b2a0-81e150228f64)
![Снимок экрана 2023-10-13 021819](https://github.com/TellEmNo/containeriztion/assets/108148686/4fb15455-43c2-4818-9cee-9f26ffe58cdb)
![Снимок экрана 2023-10-13 021829](https://github.com/TellEmNo/containeriztion/assets/108148686/4c0c56ce-f925-46c4-a57d-db96f2a4f378)
![Снимок экрана 2023-10-13 022623](https://github.com/TellEmNo/containeriztion/assets/108148686/be0f17d0-4ccb-4013-9322-635f0334516e)
![Снимок экрана 2023-10-13 022734](https://github.com/TellEmNo/containeriztion/assets/108148686/bc8e1f27-8c47-4819-8cc9-8f4397914a5a)
![Снимок экрана 2023-10-13 023231](https://github.com/TellEmNo/containeriztion/assets/108148686/73f4d7a8-cf27-4fbb-8965-a2f95b8757f0)
![Снимок экрана 2023-10-13 023600](https://github.com/TellEmNo/containeriztion/assets/108148686/39a550ed-9312-4557-8dce-d845f83812cb)
![Снимок экрана 2023-10-13 023841](https://github.com/TellEmNo/containeriztion/assets/108148686/878cf8ac-2822-403a-9a93-a5c791c6ef34)
![Снимок экрана 2023-10-13 024029](https://github.com/TellEmNo/containeriztion/assets/108148686/61cfbae9-e02f-457b-93dc-5b35bbf605c3)
![Снимок экрана 2023-10-13 024143](https://github.com/TellEmNo/containeriztion/assets/108148686/450ccbed-885a-42c3-b135-1e1716c1c9de)
![Снимок экрана 2023-10-13 024455](https://github.com/TellEmNo/containeriztion/assets/108148686/acd26d5c-0378-404d-a018-84d0d30b5ac2)
![Снимок экрана 2023-10-13 024725](https://github.com/TellEmNo/containeriztion/assets/108148686/7b3a8ad8-e488-4397-a412-48a81938c770)

##### История команд:

1. docker run -it -h GB --name gb-test ubuntu:22.10
2. ls -l /
3. ps aux
4. mkdir /example
5. ll
6. cd /example
7. touch /example/passwords.txt
8. ll
9. echo "123test" >> /example/passwords.txt
10. cat passwords.txt
11. docker ps -a
12. docker stop gb-test
13. docker start gb-test
14. docker ps -a
15. docker exec -it gb-test bash
16. ll
17. cd /example/
18. ll
19. exit
20. sudo mkdir test
21. ls
22. cd test/
23. sudo mkdir folder
24. ls
25. cd otherway/
26. touch passwords.txt
27. echo "123test" >> passwords.txt
28. cat passwords.txt
29. exit
30. cd test/folder
31. sudo nano passwd.txt
32. cat passwd.txt
33. ls
34. docker start gb-test-2
35. docker exec -it gb-test-2 bash
36. cd otherway/
37. ls
38. exit
39. ls
40. cat passwd.txt
41. cat passwords.txt
42. docker start gb-test-2
43. docker exec -it gb-test-2 bash
44. cd otherway/
45. ls
46. echo "$HOSTNAME" >> passwords.txt
47. cat passwords.txt
48. exit
49. cat passwords.txt
50. sudo nano passwords.txt
51. docker start gb-test-2
52. docker exec -it gb-test-2 bash
53. cd otherway/
54. cat passwords.txt
