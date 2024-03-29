ДЗ: Обновить ядро в базовой системе

#Версия ядра системы до обновления:
$ uname -a
Linux deb12 6.1.0-13-amd64 #1 SMP PREEMPT_DYNAMIC Debian 6.1.55-1 (2023-09-29) x86_64 GNU/Linux

#Поиск доступной версии ядра в репозитории debian
$ apt search linux-image

#Установливаем свежее ядро из ветки /stable

$ sudo apt install linux-image-6.1.0-18-amd64
```
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  firmware-linux-free linux-image-amd64
Suggested packages:
  linux-doc-6.1 debian-kernel-handbook
The following NEW packages will be installed:
  firmware-linux-free linux-image-6.1.0-18-amd64
The following packages will be upgraded:
  linux-image-amd64
1 upgraded, 2 newly installed, 0 to remove and 37 not upgraded.
Need to get 68.8 MB of archives.
After this operation, 408 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 https://deb.debian.org/debian bookworm/main amd64 firmware-linux-free all 20200122-1 [24.2 kB]
Get:2 https://deb.debian.org/debian bookworm/main amd64 linux-image-6.1.0-18-amd64 amd64 6.1.76-1 [68.8 MB]
Get:3 https://deb.debian.org/debian bookworm/main amd64 linux-image-amd64 amd64 6.1.76-1 [1476 B]      
Fetched 68.8 MB in 2min 46s (415 kB/s)                                                                 
Reading changelogs... Done
Selecting previously unselected package firmware-linux-free.
(Reading database ... 47330 files and directories currently installed.)
Preparing to unpack .../firmware-linux-free_20200122-1_all.deb ...
Unpacking firmware-linux-free (20200122-1) ...
Selecting previously unselected package linux-image-6.1.0-18-amd64.
Preparing to unpack .../linux-image-6.1.0-18-amd64_6.1.76-1_amd64.deb ...
Unpacking linux-image-6.1.0-18-amd64 (6.1.76-1) ...
Preparing to unpack .../linux-image-amd64_6.1.76-1_amd64.deb ...
Unpacking linux-image-amd64 (6.1.76-1) over (6.1.55-1) ...
Setting up linux-image-6.1.0-18-amd64 (6.1.76-1) ...
/etc/kernel/postinst.d/initramfs-tools:
update-initramfs: Generating /boot/initrd.img-6.1.0-18-amd64
W: No zstd in /usr/bin:/sbin:/bin, using gzip
/etc/kernel/postinst.d/zz-update-grub:
Generating grub configuration file ...
Found linux image: /boot/vmlinuz-6.1.0-18-amd64
Found initrd image: /boot/initrd.img-6.1.0-18-amd64
Found linux image: /boot/vmlinuz-6.1.0-13-amd64
Found initrd image: /boot/initrd.img-6.1.0-13-amd64
done
Setting up firmware-linux-free (20200122-1) ...
Setting up linux-image-amd64 (6.1.76-1) ...
Processing triggers for initramfs-tools (0.142) ...
update-initramfs: Generating /boot/initrd.img-6.1.0-18-amd64
W: No zstd in /usr/bin:/sbin:/bin, using gzip
```
Версия после обновения:
![image](https://github.com/Krug912/HJ_otus/assets/162484306/96caabea-2b78-415e-a37b-70e20a9fd7b7)
