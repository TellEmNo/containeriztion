# Контейнеризация. Семинар 2.

![Снимок экрана 2023-10-10 012050](https://github.com/TellEmNo/containeriztion/assets/108148686/9f18f6e9-f35d-4d17-9037-21f9b2cd8149)
![Снимок экрана 2023-10-10 012304](https://github.com/TellEmNo/containeriztion/assets/108148686/e4f2e5ba-d68a-482a-958c-acc38c5728ef)
![Снимок экрана 2023-10-10 012825](https://github.com/TellEmNo/containeriztion/assets/108148686/abeb1c02-7c47-437d-8e40-5ab5420091a8)
![Снимок экрана 2023-10-10 012904](https://github.com/TellEmNo/containeriztion/assets/108148686/fbc648cd-352f-49a5-98a4-d2ebe785ad61)
![Снимок экрана 2023-10-10 020107](https://github.com/TellEmNo/containeriztion/assets/108148686/c252551e-367d-4184-b98b-5f57c066259c)
![Снимок экрана 2023-10-10 020115](https://github.com/TellEmNo/containeriztion/assets/108148686/7f6c2d7a-2b71-4b20-a1be-cddd13521869)
![Снимок экрана 2023-10-10 020450](https://github.com/TellEmNo/containeriztion/assets/108148686/838d6d1c-6268-44aa-9af2-32e1b419875f)
![Снимок экрана 2023-10-10 021249](https://github.com/TellEmNo/containeriztion/assets/108148686/3415bdd0-a33e-4fb7-a3b2-dd08da337ebf)
![Снимок экрана 2023-10-10 021816](https://github.com/TellEmNo/containeriztion/assets/108148686/9433575d-9127-4da6-bf33-b27a01a527d8)
![Снимок экрана 2023-10-10 021851](https://github.com/TellEmNo/containeriztion/assets/108148686/7886f10f-f7dc-43ee-b70d-ba8ae70aaadf)
![Снимок экрана 2023-10-10 024633](https://github.com/TellEmNo/containeriztion/assets/108148686/7275c3fa-c9d4-4645-a09c-9278c229a854)
![Снимок экрана 2023-10-10 024644](https://github.com/TellEmNo/containeriztion/assets/108148686/d323863a-1a70-4aa7-bc7a-f3bcf96d53e6)
![Снимок экрана 2023-10-10 024712](https://github.com/TellEmNo/containeriztion/assets/108148686/c305340d-ced7-4e0a-8dc2-839b4203b951)
![Снимок экрана 2023-10-10 024726](https://github.com/TellEmNo/containeriztion/assets/108148686/736473ae-1bac-4e97-b169-d37197f3bb0c)

#### История команд:
 784  sudo apt install lxc debootstrap bridge-utils lxc-templates
  785  sudo apt install lxd-installer -y
  787  lxd init
  788  lxc storage list
  790  sudo apt update
  791  sudo apt upgrade
  793  sudo lxc-create -n con1 -t ubuntu
  801  sudo lxc-ls -f
  802  sudo lxc-info con1
  803  sudo lxc-start -n con1
  805  sudo lxc-attach -n con1
  806  sudo lxc-stop -n con1
  808  sudo nano /var/lib/lxc/con1/config
  809  sudo lxc-start -n con1
  810  sudo lxc-attach -n con1
  811  sudo lxc-stop -n con1
  815  sudo lxc-destroy -n con1
  824  sudo lxc-create -n con2 -t ubuntu --logfile=HomeWork02/con2.log
  825  sudo lxc-create -n con1 -t ubuntu --logfile=HomeWork02/con1.log
  826  lxc list
  827  sudo nano /var/lib/lxc/con1/config
  828  sudo nano /var/lib/lxc/con2/config
  831  sudo lxc-start con2 --logfile=/home/vlad/LXCHomeWork02/con2.log --logpriority=NOTICE
  832  sudo lxc-start con1 --logfile=/home/vlad/LXCHomeWork02/con1.log --logpriority=NOTICE
  836  sudo lxc-ls -f
  837  sudo nano /var/lib/lxc/con1/config
  838  sudo nano /var/lib/lxc/con2/config
