# Контейнеризация. Семинар 1.

### Задание: необходимо продемонстрировать изоляцию одного и того же приложения (как решено на семинаре - командного интерпретатора) в различных пространствах имен.

![Снимок экрана 2023-10-06 033613](https://github.com/TellEmNo/containeriztion/assets/108148686/6ef0b888-222f-4563-8fbf-baa5fb315a50)
![Снимок экрана 2023-10-06 033648](https://github.com/TellEmNo/containeriztion/assets/108148686/251c8518-7706-4995-9c1a-032e8f3d6dd2)
![Снимок экрана 2023-10-06 033751](https://github.com/TellEmNo/containeriztion/assets/108148686/6702afa5-2fb9-450e-b678-74e327260d55)
![Снимок экрана 2023-10-06 033825](https://github.com/TellEmNo/containeriztion/assets/108148686/47c63f18-e490-4779-ace0-7a5420f55470)

#### История команд:
733  mkdir testfolder
  734  ls
  735  cd testfolder/
  736  mkdir bin
  737  ls
  738  sudo cp /bin/bash ~/test/testfolder/bin/
  739  cd bin
  740  ls
  741  cd ..
  742  cd bin/
  743  ldd /bin/bash
  744  mkdir ~/test/testfolder/lib ~/test/testfolder/lib64
  745  cd ..
  746  ls
  747  cp /lib/x86_64-linux-gnu/libtinfo.so.6 ~/test/testfolder/lib
  748  cp /lib/x86_64-linux-gnu/libc.so.6 ~/test/testfolder/lib
  749  cp /lib64/ld-linux-x86-64.so.2 ~/test/testfolder/lib64/
  750  cd lib
  751  ls
  752  cd ..
  753  tree
  754  cd bin/
  755  sudo chroot ~/test/testfolder/bin/bash
  756  sudo chroot ~/test/testfolder/
  757  cp /lib/x86_64-linux-gnu/libc.so ~/test/testfolder/lib
  758  cd ..
  759  tree
  760  sudo chroot ~/test/testfolder/
  761  history
  762  sudo chroot ~/test/testfolder/
  763  tree
  764  ps aux
  765  ps head
  766  ps aux | head
  767  ip netns add testns
  768  cd
  769  ip
  770  ip a
  771  sudo ip netns add testns
  772  ip a
  773  sudo ip netns exec testns bash
  774  ls
  775  ip a
  776  unshare --net --pid --fork --mount-proc /bin/bash
  777  sudo unshare --net --pid --fork --mount-proc /bin/bash
