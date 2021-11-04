
rusud@LAPTOP-TQCORJEG MINGW64 ~
$ ssh -i ~/.ssh/id_rsa ec2-user@18.196.90.105
Last login: Thu Nov  4 13:35:16 2021 from 130-0-43-75.broadband.tenet.odessa.ua

       __|  __|_  )
       _|  (     /   Amazon Linux 2 AMI
      ___|\___|___|

https://aws.amazon.com/amazon-linux-2/
[ec2-user@ip-172-31-44-146 ~]$  find /opt -type f -name "script.*" -print -exec ls -la {} \;
/opt/Asya/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 66 Nov  3 12:47 /opt/Asya/script.sh
/opt/hanuliak/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 63 Nov  3 12:44 /opt/hanuliak/script.sh
/opt/Nina/script.sh
-rw-rw-r-- 1 ec2-user ec2-user 36 Nov  3 12:35 /opt/Nina/script.sh
/opt/Dima/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 36 Nov  1 12:37 /opt/Dima/script.sh
/opt/Natalia/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 71 Nov  3 12:54 /opt/Natalia/script.sh
/opt/Viktoria/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 70 Nov  3 12:41 /opt/Viktoria/script.sh
/opt/Alex/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 36 Nov  1 13:06 /opt/Alex/script.sh
/opt/Viktor/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 36 Nov  1 12:48 /opt/Viktor/script.sh
/opt/Wlad/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 69 Nov  3 12:36 /opt/Wlad/script.sh
/opt/Vladimir/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 67 Nov  3 12:56 /opt/Vladimir/script.sh
/opt/Oleg/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 36 Nov  2 14:20 /opt/Oleg/script.sh
/opt/Mirlan/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 69 Nov  3 12:47 /opt/Mirlan/script.sh
/opt/Ndrew/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 70 Nov  3 12:39 /opt/Ndrew/script.sh
/opt/Daria/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 68 Nov  3 12:39 /opt/Daria/script.sh
/opt/AlexDir/script.sh
-rw-rw-r-- 1 ec2-user ec2-user 36 Nov  1 13:03 /opt/AlexDir/script.sh
/opt/Alexandra/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 73 Nov  3 12:39 /opt/Alexandra/script.sh
/opt/Dmitri/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 36 Nov  1 13:02 /opt/Dmitri/script.sh
/opt/Alena/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 69 Nov  3 12:41 /opt/Alena/script.sh
/opt/Kateryna/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 76 Nov  3 13:29 /opt/Kateryna/script.sh
/opt/Valeri/script.sh
-rwxrw-r-- 1 ec2-user ec2-user 71 Nov  3 12:46 /opt/Valeri/script.sh
[ec2-user@ip-172-31-44-146 ~]$ pwd
/home/ec2-user
[ec2-user@ip-172-31-44-146 ~]$ cd /opt
[ec2-user@ip-172-31-44-146 opt]$ pwd
/opt
[ec2-user@ip-172-31-44-146 opt]$ crontab -e
crontab: installing new crontab
[ec2-user@ip-172-31-44-146 opt]$ crontab -l
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Asya/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.ch >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Nina/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Natalia/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktoria/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alex/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktor/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Wlad/script.sh >> /opt/Wlad/log.txt
0 12 * * * /opt/Vladimir/script.sh >> /opt/Vladimir/log.txt
* * * * * /opt/Oleg/script.sh >> /opt/Oleg/log.txt
#* * * * * /opt/Mirlan/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Daria/script.sh >> /opt/Daria/log.txt
#* * * * * /opt/AlexDir/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alexandra/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dmitri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Alena/script.sh >> /opt/Alena/log.txt
#* * * * * /opt/Kateryna/script.sh >> /opt/Kateryna/log.txt
#* * * * * /opt/leri/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >>/opt/Dima/log.txt


[ec2-user@ip-172-31-44-146 opt]$ crontab -lu ec2-user
must be privileged to use -u
[ec2-user@ip-172-31-44-146 opt]$ ls
Alena  Alex  Alexandra  alexdir  AlexDir  Asya  aws  Daria  Dima  Dmitri  hanuliak  Kateryna  Lena  Mirlan  Natalia  Ndrew  Nina  Oleg  rh  Valeri  Viktor  Viktoria  Vladimir  Wlad
[ec2-user@ip-172-31-44-146 opt]$ tail log.txt
tail: cannot open ‘log.txt’ for reading: No such file or directory
[ec2-user@ip-172-31-44-146 opt]$ pwd
/opt
[ec2-user@ip-172-31-44-146 opt]$ cd Dima
[ec2-user@ip-172-31-44-146 Dima]$ ls
script.sh
[ec2-user@ip-172-31-44-146 Dima]$ cronta -e
-bash: cronta: command not found
[ec2-user@ip-172-31-44-146 Dima]$ cd ..
[ec2-user@ip-172-31-44-146 opt]$ cronta -e
-bash: cronta: command not found
[ec2-user@ip-172-31-44-146 opt]$ crontab -l
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Asya/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.ch >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Nina/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Natalia/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktoria/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alex/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktor/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Wlad/script.sh >> /opt/Wlad/log.txt
5 * * * * /opt/Vladimir/script.sh >> /opt/Vladimir/log.txt
* * * * * /opt/Oleg/script.sh >> /opt/Oleg/log.txt
#* * * * * /opt/Mirlan/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Daria/script.sh >> /opt/Daria/log.txt
#* * * * * /opt/AlexDir/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alexandra/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dmitri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Alena/script.sh >> /opt/Alena/log.txt
#* * * * * /opt/Kateryna/script.sh >> /opt/Kateryna/log.txt
#* * * * * /opt/leri/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >>/opt/Dima/log.txt


[ec2-user@ip-172-31-44-146 opt]$ crontab -e
crontab: installing new crontab
[ec2-user@ip-172-31-44-146 opt]$ cd Dima
[ec2-user@ip-172-31-44-146 Dima]$ ls
script.sh
[ec2-user@ip-172-31-44-146 Dima]$ crontab -e
crontab: no changes made to crontab
[ec2-user@ip-172-31-44-146 Dima]$ crontab -l
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Asya/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.ch >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Nina/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Natalia/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktoria/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alex/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktor/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Wlad/script.sh >> /opt/Wlad/log.txt
5 * * * * /opt/Vladimir/script.sh >> /opt/Vladimir/log.txt
* * * * * /opt/Oleg/script.sh >> /opt/Oleg/log.txt
#* * * * * /opt/Mirlan/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Daria/script.sh >> /opt/Daria/log.txt
#* * * * * /opt/AlexDir/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alexandra/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dmitri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Alena/script.sh >> /opt/Alena/log.txt
#* * * * * /opt/Kateryna/script.sh >> /opt/Kateryna/log.txt
#* * * * * /opt/leri/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >> /opt/Dima/log.txt


[ec2-user@ip-172-31-44-146 Dima]$ pwd
/opt/Dima
[ec2-user@ip-172-31-44-146 Dima]$ ls
script.sh
[ec2-user@ip-172-31-44-146 Dima]$ crontab -e
crontab: installing new crontab
[ec2-user@ip-172-31-44-146 Dima]$ ls
script.sh
[ec2-user@ip-172-31-44-146 Dima]$ crontab -l
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Asya/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.ch >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Nina/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Natalia/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktoria/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alex/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktor/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Wlad/script.sh >> /opt/Wlad/log.txt
0 * * * * /opt/Vladimir/script.sh >> /opt/Vladimir/log.txt
* * * * * /opt/Oleg/script.sh >> /opt/Oleg/log.txt
#* * * * * /opt/Mirlan/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Daria/script.sh >> /opt/Daria/log.txt
#* * * * * /opt/AlexDir/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alexandra/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dmitri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Alena/script.sh >> /opt/Alena/log.txt
#* * * * * /opt/Kateryna/script.sh >> /opt/Kateryna/log.txt
#* * * * * /opt/leri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Dima/script.sh >> /opt/Dima/log.txt


[ec2-user@ip-172-31-44-146 Dima]$ crontab -l
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Asya/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.ch >> /opt/Ndrew/log.txt
#* * * * * /opt/hanuliak/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Nina/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dima/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Natalia/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktoria/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alex/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Viktor/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Wlad/script.sh >> /opt/Wlad/log.txt
0 * * * * /opt/Vladimir/script.sh >> /opt/Vladimir/log.txt
* * * * * /opt/Oleg/script.sh >> /opt/Oleg/log.txt
#* * * * * /opt/Mirlan/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Ndrew/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Daria/script.sh >> /opt/Daria/log.txt
#* * * * * /opt/AlexDir/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Alexandra/script.sh >> /opt/Ndrew/log.txt
#* * * * * /opt/Dmitri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Alena/script.sh >> /opt/Alena/log.txt
#* * * * * /opt/Kateryna/script.sh >> /opt/Kateryna/log.txt
#* * * * * /opt/leri/script.sh >> /opt/Ndrew/log.txt
* * * * * /opt/Dima/script.sh >> /opt/Dima/log.txt


[ec2-user@ip-172-31-44-146 Dima]$ ls
log.txt  script.sh
[ec2-user@ip-172-31-44-146 Dima]$ vi script.sh
[ec2-user@ip-172-31-44-146 Dima]$ ./script.sh
Thu Nov  4 15:14:11 UTC 2021
it works!
Hello Dima !
[ec2-user@ip-172-31-44-146 Dima]$ cat ./script.sh
#!/bin/bash
USER=Dima


date
 echo "it works!"
 echo Hello $USER !
[ec2-user@ip-172-31-44-146 Dima]$ cat ./log.txt
Thu Nov  4 14:36:01 UTC 2021
it works!
Thu Nov  4 14:37:01 UTC 2021
it works!
Thu Nov  4 14:38:01 UTC 2021
it works!
Thu Nov  4 14:39:01 UTC 2021
it works!
Thu Nov  4 14:40:01 UTC 2021
it works!
Thu Nov  4 14:41:01 UTC 2021
it works!
Thu Nov  4 14:42:01 UTC 2021
it works!
Thu Nov  4 14:43:02 UTC 2021
it works!
Thu Nov  4 14:44:01 UTC 2021
it works!
Thu Nov  4 14:45:01 UTC 2021
it works!
Thu Nov  4 14:46:01 UTC 2021
it works!
Thu Nov  4 14:47:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:48:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:49:02 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:50:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:51:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:52:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:53:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:54:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:55:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:56:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:57:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:58:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 14:59:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:00:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:01:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:02:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:03:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:04:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:05:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:06:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:07:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:08:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:09:02 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:10:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:11:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:12:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:13:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:14:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:15:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:16:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:17:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:18:02 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:19:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:20:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:21:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:22:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:23:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:24:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:25:01 UTC 2021
it works!
Hello Dima !
[ec2-user@ip-172-31-44-146 Dima]$ tai -f /opt/Dima/log.txt
-bash: tai: command not found
[ec2-user@ip-172-31-44-146 Dima]$ tail -f /opt/Dima/log.txt
Hello Dima !
Thu Nov  4 15:26:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:27:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:28:01 UTC 2021
it works!
Hello Dima !
Thu Nov  4 15:29:01 UTC 2021
it works!
Hello Dima !
^[[A^[[A^[[B^[[A^[[A^[[B^[[A^[[B^[[A^[^[^[^[^[^[^[^L^[[D^[[C^[i^[
:x
Thu Nov  4 15:30:01 UTC 2021
it works!
Hello Dima !
^C
[ec2-user@ip-172-31-44-146 Dima]$ tail -f /opt/Dima/log.txt | grep hello
^[[A^[[A^[[B^[[B^C
[ec2-user@ip-172-31-44-146 Dima]$ ps -ef
UID        PID  PPID  C STIME TTY          TIME CMD
root         1     0  0 Oct27 ?        00:00:38 /usr/lib/systemd/systemd --switched-root --system --deserialize 21
root         2     0  0 Oct27 ?        00:00:00 [kthreadd]
root         4     2  0 Oct27 ?        00:00:00 [kworker/0:0H]
root         6     2  0 Oct27 ?        00:00:00 [mm_percpu_wq]
root         7     2  0 Oct27 ?        00:00:01 [ksoftirqd/0]
root         8     2  0 Oct27 ?        00:00:06 [rcu_sched]
root         9     2  0 Oct27 ?        00:00:00 [rcu_bh]
root        10     2  0 Oct27 ?        00:00:00 [migration/0]
root        11     2  0 Oct27 ?        00:00:01 [watchdog/0]
root        12     2  0 Oct27 ?        00:00:00 [cpuhp/0]
root        13     2  0 Oct27 ?        00:00:00 [cpuhp/1]
root        14     2  0 Oct27 ?        00:00:01 [watchdog/1]
root        15     2  0 Oct27 ?        00:00:00 [migration/1]
root        16     2  0 Oct27 ?        00:00:00 [ksoftirqd/1]
root        18     2  0 Oct27 ?        00:00:00 [kworker/1:0H]
root        20     2  0 Oct27 ?        00:00:00 [kdevtmpfs]
root        21     2  0 Oct27 ?        00:00:00 [netns]
root       112     2  0 Oct27 ?        00:00:00 [khungtaskd]
root       143     2  0 Oct27 ?        00:00:00 [oom_reaper]
root       174     2  0 Oct27 ?        00:00:00 [writeback]
root       188     2  0 Oct27 ?        00:00:00 [kcompactd0]
root       189     2  0 Oct27 ?        00:00:00 [ksmd]
root       190     2  0 Oct27 ?        00:00:00 [khugepaged]
root       191     2  0 Oct27 ?        00:00:00 [crypto]
root       192     2  0 Oct27 ?        00:00:00 [kintegrityd]
root       193     2  0 Oct27 ?        00:00:00 [kblockd]
root       301     2  0 Oct27 ?        00:00:00 [md]
root       305     2  0 Oct27 ?        00:00:00 [edac-poller]
root       310     2  0 Oct27 ?        00:00:00 [watchdogd]
root       434     2  0 Oct27 ?        00:00:01 [kauditd]
root       440     2  0 Oct27 ?        00:00:00 [kswapd0]
root       572     2  0 Oct27 ?        00:00:00 [kthrotld]
root       617     2  0 Oct27 ?        00:00:00 [kstrp]
root       642     2  0 Oct27 ?        00:00:00 [ipv6_addrconf]
root      1015     2  0 Oct27 ?        00:00:00 [nvme-wq]
root      1056     2  0 Oct27 ?        00:00:00 [xfsalloc]
root      1057     2  0 Oct27 ?        00:00:00 [xfs_mru_cache]
root      1060     2  0 Oct27 ?        00:00:00 [xfs-buf/nvme0n1]
root      1061     2  0 Oct27 ?        00:00:00 [xfs-data/nvme0n]
root      1062     2  0 Oct27 ?        00:00:00 [xfs-conv/nvme0n]
root      1063     2  0 Oct27 ?        00:00:00 [xfs-cil/nvme0n1]
root      1064     2  0 Oct27 ?        00:00:00 [xfs-reclaim/nvm]
root      1065     2  0 Oct27 ?        00:00:00 [xfs-log/nvme0n1]
root      1066     2  0 Oct27 ?        00:00:00 [xfs-eofblocks/n]
root      1067     2  0 Oct27 ?        00:01:34 [xfsaild/nvme0n1]
root      1068     2  0 Oct27 ?        00:00:00 [kworker/0:1H]
root      1129     1  0 Oct27 ?        00:00:16 /usr/lib/systemd/systemd-journald
root      1153     2  0 Oct27 ?        00:00:00 [ena]
root      1159     1  0 Oct27 ?        00:00:00 /usr/sbin/lvmetad -f
root      1173     1  0 Oct27 ?        00:00:00 /usr/lib/systemd/systemd-udevd
root      1654     2  0 Oct27 ?        00:00:00 [rpciod]
root      1655     2  0 Oct27 ?        00:00:00 [xprtiod]
root      1659     1  0 Oct27 ?        00:00:03 /sbin/auditd
root      1689     1  0 Oct27 ?        00:00:13 /usr/sbin/irqbalance --foreground
root      1693     1  0 Oct27 ?        00:00:13 /usr/lib/systemd/systemd-logind
libstor+  1694     1  0 Oct27 ?        00:00:01 /usr/bin/lsmd -d
dbus      1696     1  0 Oct27 ?        00:00:24 /usr/bin/dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation
rpc       1698     1  0 Oct27 ?        00:00:00 /sbin/rpcbind -w
rngd      1706     1  0 Oct27 ?        00:00:08 /sbin/rngd -f --fill-watermark=0 --exclude=jitter
chrony    1720     1  0 Oct27 ?        00:00:06 /usr/sbin/chronyd
root      1724     1  0 Oct27 ?        00:00:00 /usr/sbin/gssproxy -D
root      1911     2  0 Oct27 ?        00:00:01 [kworker/1:1H]
root      1929     1  0 Oct27 ?        00:00:00 /sbin/dhclient -q -lf /var/lib/dhclient/dhclient--eth0.lease -pf /var/run/dhclient-eth0.pid eth0
root      1974     1  0 Oct27 ?        00:00:00 /sbin/dhclient -6 -nw -lf /var/lib/dhclient/dhclient6--eth0.lease -pf /var/run/dhclient6-eth0.pid eth0
root      2123     1  0 Oct27 ?        00:00:01 /usr/libexec/postfix/master -w
postfix   2126  2123  0 Oct27 ?        00:00:00 qmgr -l -t unix -u
root      2173     1  0 Oct27 ?        00:00:33 /usr/sbin/rsyslogd -n
root      2175     1  0 Oct27 ?        00:00:26 /usr/bin/amazon-ssm-agent
root      2203     1  0 Oct27 ?        00:00:00 /usr/sbin/atd -f
root      2218     1  0 Oct27 tty1     00:00:00 /sbin/agetty --noclear tty1 linux
root      2219     1  0 Oct27 ttyS0    00:00:00 /sbin/agetty --keep-baud 115200,38400,9600 ttyS0 vt220
root      2339     1  0 Oct27 ?        00:00:02 /usr/sbin/sshd -D
root      2352  2175  0 Oct27 ?        00:00:20 /usr/bin/ssm-agent-worker
root      2423     1  0 Oct27 ?        00:00:00 /usr/sbin/acpid
root      2840     2  0 13:48 ?        00:00:00 [kworker/u4:0]
root      3726  2339  0 14:00 ?        00:00:00 sshd: ec2-user [priv]
ec2-user  3728  3726  0 14:00 ?        00:00:00 sshd: ec2-user@pts/1
ec2-user  3729  3728  0 14:01 pts/1    00:00:00 -bash
root      5653     2  0 14:25 ?        00:00:00 [kworker/u4:2]
postfix   7067  2123  0 14:43 ?        00:00:00 pickup -l -t unix -u
root      8919     2  0 15:07 ?        00:00:00 [kworker/1:2]
root      9595     2  0 15:16 ?        00:00:00 [kworker/0:1]
root     10279     2  0 15:25 ?        00:00:00 [kworker/0:0]
root     10695     2  0 15:30 ?        00:00:00 [kworker/1:0]
root     10849     2  0 15:32 ?        00:00:00 [kworker/0:2]
root     11221     2  0 15:37 ?        00:00:00 [kworker/1:1]
root     11296     2  0 15:38 ?        00:00:00 [kworker/0:3]
ec2-user 11311  3729  0 15:38 pts/1    00:00:00 ps -ef
root     22827     1  0 Nov03 ?        00:00:01 /usr/sbin/crond -n
[ec2-user@ip-172-31-44-146 Dima]$ top
top - 15:40:05 up 8 days,  3:53,  4 users,  load average: 0.00, 0.00, 0.00
Tasks:  92 total,   1 running,  50 sleeping,   0 stopped,   0 zombie
%Cpu(s):  0.2 us,  0.0 sy,  0.0 ni, 99.8 id,  0.0 wa,  0.0 hi,  0.0 si,  0.0 st
KiB Mem :   979940 total,   265588 free,   119960 used,   594392 buff/cache
KiB Swap:        0 total,        0 free,        0 used.   696756 avail Mem

  PID USER      PR  NI    VIRT    RES    SHR S  %CPU %MEM     TIME+ COMMAND
    1 root      20   0  125688   5660   3980 S   0.0  0.6   0:38.66 systemd
    2 root      20   0       0      0      0 S   0.0  0.0   0:00.11 kthreadd
    4 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 kworker/0:0H
    6 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 mm_percpu_wq
    7 root      20   0       0      0      0 S   0.0  0.0   0:01.08 ksoftirqd/0
    8 root      20   0       0      0      0 I   0.0  0.0   0:06.97 rcu_sched
    9 root      20   0       0      0      0 I   0.0  0.0   0:00.00 rcu_bh
   10 root      rt   0       0      0      0 S   0.0  0.0   0:00.07 migration/0
   11 root      rt   0       0      0      0 S   0.0  0.0   0:01.39 watchdog/0
   12 root      20   0       0      0      0 S   0.0  0.0   0:00.00 cpuhp/0
   13 root      20   0       0      0      0 S   0.0  0.0   0:00.00 cpuhp/1
   14 root      rt   0       0      0      0 S   0.0  0.0   0:01.23 watchdog/1
   15 root      rt   0       0      0      0 S   0.0  0.0   0:00.07 migration/1
   16 root      20   0       0      0      0 S   0.0  0.0   0:00.83 ksoftirqd/1
   18 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 kworker/1:0H
   20 root      20   0       0      0      0 S   0.0  0.0   0:00.00 kdevtmpfs
   21 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 netns
  112 root      20   0       0      0      0 S   0.0  0.0   0:00.20 khungtaskd
  143 root      20   0       0      0      0 S   0.0  0.0   0:00.00 oom_reaper
  174 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 writeback
  188 root      20   0       0      0      0 S   0.0  0.0   0:00.00 kcompactd0
  189 root      25   5       0      0      0 S   0.0  0.0   0:00.00 ksmd
  190 root      39  19       0      0      0 S   0.0  0.0   0:00.00 khugepaged
  191 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 crypto
  192 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 kintegrityd
  193 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 kblockd
  301 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 md
  305 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 edac-poller
  310 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 watchdogd
  434 root      20   0       0      0      0 S   0.0  0.0   0:01.21 kauditd
  440 root      20   0       0      0      0 S   0.0  0.0   0:00.15 kswapd0
  572 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 kthrotld
  617 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 kstrp
  642 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 ipv6_addrconf
 1015 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 nvme-wq
 1056 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfsalloc
 1057 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs_mru_cache
 1060 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-buf/nvme0n1
 1061 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-data/nvme0n
 1062 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-conv/nvme0n
 1063 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-cil/nvme0n1
 1064 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-reclaim/nvm
 1065 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-log/nvme0n1
 1066 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xfs-eofblocks/n
 1067 root      20   0       0      0      0 S   0.0  0.0   1:34.82 xfsaild/nvme0n1
 1068 root       0 -20       0      0      0 I   0.0  0.0   0:00.83 kworker/0:1H
 1129 root      20   0   47156  10200   9864 S   0.0  1.0   0:16.70 systemd-journal
 1153 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 ena
 1159 root      20   0  118800   2164   1892 S   0.0  0.2   0:00.00 lvmetad
 1173 root      20   0   46040   3444   2672 S   0.0  0.4   0:00.03 systemd-udevd
 1654 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 rpciod
 1655 root       0 -20       0      0      0 I   0.0  0.0   0:00.00 xprtiod
[ec2-user@ip-172-31-44-146 Dima]$ ps -ef
UID        PID  PPID  C STIME TTY          TIME CMD
root         1     0  0 Oct27 ?        00:00:38 /usr/lib/systemd/systemd --switched-root --system --deserialize 21
root         2     0  0 Oct27 ?        00:00:00 [kthreadd]
root         4     2  0 Oct27 ?        00:00:00 [kworker/0:0H]
root         6     2  0 Oct27 ?        00:00:00 [mm_percpu_wq]
root         7     2  0 Oct27 ?        00:00:01 [ksoftirqd/0]
root         8     2  0 Oct27 ?        00:00:06 [rcu_sched]
root         9     2  0 Oct27 ?        00:00:00 [rcu_bh]
root        10     2  0 Oct27 ?        00:00:00 [migration/0]
root        11     2  0 Oct27 ?        00:00:01 [watchdog/0]
root        12     2  0 Oct27 ?        00:00:00 [cpuhp/0]
root        13     2  0 Oct27 ?        00:00:00 [cpuhp/1]
root        14     2  0 Oct27 ?        00:00:01 [watchdog/1]
root        15     2  0 Oct27 ?        00:00:00 [migration/1]
root        16     2  0 Oct27 ?        00:00:00 [ksoftirqd/1]
root        18     2  0 Oct27 ?        00:00:00 [kworker/1:0H]
root        20     2  0 Oct27 ?        00:00:00 [kdevtmpfs]
root        21     2  0 Oct27 ?        00:00:00 [netns]
root       112     2  0 Oct27 ?        00:00:00 [khungtaskd]
root       143     2  0 Oct27 ?        00:00:00 [oom_reaper]
root       174     2  0 Oct27 ?        00:00:00 [writeback]
root       188     2  0 Oct27 ?        00:00:00 [kcompactd0]
root       189     2  0 Oct27 ?        00:00:00 [ksmd]
root       190     2  0 Oct27 ?        00:00:00 [khugepaged]
root       191     2  0 Oct27 ?        00:00:00 [crypto]
root       192     2  0 Oct27 ?        00:00:00 [kintegrityd]
root       193     2  0 Oct27 ?        00:00:00 [kblockd]
root       301     2  0 Oct27 ?        00:00:00 [md]
root       305     2  0 Oct27 ?        00:00:00 [edac-poller]
root       310     2  0 Oct27 ?        00:00:00 [watchdogd]
root       434     2  0 Oct27 ?        00:00:01 [kauditd]
root       440     2  0 Oct27 ?        00:00:00 [kswapd0]
root       572     2  0 Oct27 ?        00:00:00 [kthrotld]
root       617     2  0 Oct27 ?        00:00:00 [kstrp]
root       642     2  0 Oct27 ?        00:00:00 [ipv6_addrconf]
root      1015     2  0 Oct27 ?        00:00:00 [nvme-wq]
root      1056     2  0 Oct27 ?        00:00:00 [xfsalloc]
root      1057     2  0 Oct27 ?        00:00:00 [xfs_mru_cache]
root      1060     2  0 Oct27 ?        00:00:00 [xfs-buf/nvme0n1]
root      1061     2  0 Oct27 ?        00:00:00 [xfs-data/nvme0n]
root      1062     2  0 Oct27 ?        00:00:00 [xfs-conv/nvme0n]
root      1063     2  0 Oct27 ?        00:00:00 [xfs-cil/nvme0n1]
root      1064     2  0 Oct27 ?        00:00:00 [xfs-reclaim/nvm]
root      1065     2  0 Oct27 ?        00:00:00 [xfs-log/nvme0n1]
root      1066     2  0 Oct27 ?        00:00:00 [xfs-eofblocks/n]
root      1067     2  0 Oct27 ?        00:01:34 [xfsaild/nvme0n1]
root      1068     2  0 Oct27 ?        00:00:00 [kworker/0:1H]
root      1129     1  0 Oct27 ?        00:00:16 /usr/lib/systemd/systemd-journald
root      1153     2  0 Oct27 ?        00:00:00 [ena]
root      1159     1  0 Oct27 ?        00:00:00 /usr/sbin/lvmetad -f
root      1173     1  0 Oct27 ?        00:00:00 /usr/lib/systemd/systemd-udevd
root      1654     2  0 Oct27 ?        00:00:00 [rpciod]
root      1655     2  0 Oct27 ?        00:00:00 [xprtiod]
root      1659     1  0 Oct27 ?        00:00:03 /sbin/auditd
root      1689     1  0 Oct27 ?        00:00:13 /usr/sbin/irqbalance --foreground
root      1693     1  0 Oct27 ?        00:00:13 /usr/lib/systemd/systemd-logind
libstor+  1694     1  0 Oct27 ?        00:00:01 /usr/bin/lsmd -d
dbus      1696     1  0 Oct27 ?        00:00:24 /usr/bin/dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation
rpc       1698     1  0 Oct27 ?        00:00:00 /sbin/rpcbind -w
rngd      1706     1  0 Oct27 ?        00:00:08 /sbin/rngd -f --fill-watermark=0 --exclude=jitter
chrony    1720     1  0 Oct27 ?        00:00:06 /usr/sbin/chronyd
root      1724     1  0 Oct27 ?        00:00:00 /usr/sbin/gssproxy -D
root      1911     2  0 Oct27 ?        00:00:01 [kworker/1:1H]
root      1929     1  0 Oct27 ?        00:00:00 /sbin/dhclient -q -lf /var/lib/dhclient/dhclient--eth0.lease -pf /var/run/dhclient-eth0.pid eth0
root      1974     1  0 Oct27 ?        00:00:00 /sbin/dhclient -6 -nw -lf /var/lib/dhclient/dhclient6--eth0.lease -pf /var/run/dhclient6-eth0.pid eth0
root      2123     1  0 Oct27 ?        00:00:01 /usr/libexec/postfix/master -w
postfix   2126  2123  0 Oct27 ?        00:00:00 qmgr -l -t unix -u
root      2173     1  0 Oct27 ?        00:00:33 /usr/sbin/rsyslogd -n
root      2175     1  0 Oct27 ?        00:00:26 /usr/bin/amazon-ssm-agent
root      2203     1  0 Oct27 ?        00:00:00 /usr/sbin/atd -f
root      2218     1  0 Oct27 tty1     00:00:00 /sbin/agetty --noclear tty1 linux
root      2219     1  0 Oct27 ttyS0    00:00:00 /sbin/agetty --keep-baud 115200,38400,9600 ttyS0 vt220
root      2339     1  0 Oct27 ?        00:00:02 /usr/sbin/sshd -D
root      2352  2175  0 Oct27 ?        00:00:20 /usr/bin/ssm-agent-worker
root      2423     1  0 Oct27 ?        00:00:00 /usr/sbin/acpid
root      2840     2  0 13:48 ?        00:00:00 [kworker/u4:0]
root      3726  2339  0 14:00 ?        00:00:00 sshd: ec2-user [priv]
ec2-user  3728  3726  0 14:00 ?        00:00:00 sshd: ec2-user@pts/1
ec2-user  3729  3728  0 14:01 pts/1    00:00:00 -bash
root      5653     2  0 14:25 ?        00:00:00 [kworker/u4:2]
postfix   7067  2123  0 14:43 ?        00:00:00 pickup -l -t unix -u
root      8919     2  0 15:07 ?        00:00:00 [kworker/1:2]
root      9595     2  0 15:16 ?        00:00:00 [kworker/0:1]
root     10279     2  0 15:25 ?        00:00:00 [kworker/0:0]
root     10695     2  0 15:30 ?        00:00:00 [kworker/1:0]
root     10849     2  0 15:32 ?        00:00:00 [kworker/0:2]
root     11221     2  0 15:37 ?        00:00:00 [kworker/1:1]
root     11296     2  0 15:38 ?        00:00:00 [kworker/0:3]
root     11318  2339  0 15:38 ?        00:00:00 sshd: [accepted]
sshd     11321 11318  0 15:38 ?        00:00:00 sshd: [net]
root     11375     2  0 15:39 ?        00:00:00 [kworker/1:3]
ec2-user 11469  3729  0 15:40 pts/1    00:00:00 ps -ef
root     22827     1  0 Nov03 ?        00:00:01 /usr/sbin/crond -n
[ec2-user@ip-172-31-44-146 Dima]$ ps -ef | wc -l
93
[ec2-user@ip-172-31-44-146 Dima]$ ps -ef | grep ssh
root      2339     1  0 Oct27 ?        00:00:02 /usr/sbin/sshd -D
root      3726  2339  0 14:00 ?        00:00:00 sshd: ec2-user [priv]
ec2-user  3728  3726  0 14:00 ?        00:00:00 sshd: ec2-user@pts/1
ec2-user 17023  3729  0 16:52 pts/1    00:00:00 grep --color=auto ssh
[ec2-user@ip-172-31-44-146 Dima]$ vi ./script.sh
[ec2-user@ip-172-31-44-146 Dima]$ contab -e
-bash: contab: command not found
[ec2-user@ip-172-31-44-146 Dima]$ crontab -e
crontab: installing new crontab
[ec2-user@ip-172-31-44-146 Dima]$
