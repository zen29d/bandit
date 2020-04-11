# bandit
| Level |Key  |Hint|Command|
|--|--|---|----|
| level0 | bandit0 | |``cat readme`` |
| level1 | boJ9jbbUNNfktd78OOpsqOltutMc3MY1 | show dashed file | ``cat ./-`` |
| level2 | CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9 | spaced file name | ``cat 'spaces in this filename'`` |
| level3 | UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK | hidden file | ``cat inhere/.hidden`` |
| level4 | pIwrPrtPN36QITSp3EQaw936yaFoFgAB | find ascii file | ``file ./* \| grep ASCII`` <br>``cat inhere/-file07 ``|
| level5 | koReBOKuIDDepwhWk7jZC0RTdopnAYKh | *find file with size | ``ls -l $(find ./ -type f) \| grep '1033'`` <br>``cat inhere/maybehere07/.file2 ``|
| level6 | DXjZPULLxYr17uwoI01bNLQbtFemEgo7 | *find file with user | ``find / -print -ls \| grep 'bandit7'``<br> ``cat /var/lib/dpkg/info/bandit7.password`` |
| level7 | HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs | find word | ``cat data.txt \| grep millionth`` |
| level8 | cvX2JJa4CFALtqS87jk27qwqGhBM9plV | find non-repeated | ``sort data.txt \| uniq -u`` |
| level9 | UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR | find words | ``strings data.txt \| grep '='`` |
| level10 | truKLdjsbJ5g7yyJ2X2R0o3a5HQJFuLk | decode data | ``base64 -d data.txt``|
| levle11 | IFukwKGsFW8MOq3IRFqrxE1hxTNEbUPR | decipher data | ``cat data.txt \| tr 'a-zA-Z' 'n-za-mN-ZA-M'``|
| level12 | 5Te8Y4drgCRfCx8ugdwuEX8KFC6k2EUu | convert, extract data | ``xxd -r data.txt hello.bin``<br>``zcat hello.bin \| bzcat \| zcat \| tar xO \| tar xO \| bzcat \| tar xO \| zcat \| file - ``|
| level13 | 8ZjyCRiBWFYkneahHwxCv3wb2a1ORpYL | save sshkey to host | ``cat sshkey.private``<br> ``(login level14: chmod 600 <sshkey> && ssh -i <sshkey> host@machine)`` |
| level14 | 4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e | telnet | ``telnet localhost 30000 (input l14 key)``<br>``(l14 key: cat /etc/bandit_pass/bandit14) ``|
| level15 | BfMYroe26WYalil77FoDi9qh59eK5xNr | ssh with ssl | ``openssl s_client -connect localhost:30001 (paste current level key) ``|
| level16 | cluFn7wTiGryunymYOu4RcffSxQluehd | find port, ssh ssl | ``nmap -p31000-32000 localhost``<br>`` openssl s_client -connect localhost:<port> (paste l16 key)``<br>`` ssh l17 ``|
| level17 | xLYVMN9WE5zQ5vHacb0sZEVqbrp7nBTn | find difference | ``diff passwords.new passwords.old (l17 key: cat /etc/bandit_pass/bandit17) ``|
| level18 | kfBf3eYk5BPBRzwjqutbbfE887SVc5Yd | ssh with cmd | ``ssh -p 2220 bandit18@bandit.labs.overthewire.org cat readme ``|
| level19 | IueksS7Ubh8G3DCwVzrTd8rAVOwq3M5x | |``./bandit20-do cat /etc/bandit_pass/bandit20 ``|
| level20 | GbKksEFF4yrVs6il55v6gwY5aVje5f0j | two ssh for ser,cli | ``nc -lp 1213 (paste l20 key)``<br>`` (in other terminal) ./suconnect 1213`` |
| level21 | gE269g2h3mw3pwgrj0Ha9Uoqen1c9DGr | | ``cat /etc/cron.d/cronjob_bandit22``<br>``cat /usr/bin/cronjob_bandit22.sh``<br>``cat /tmp/<tmp_new_dir> ``|
| level22 | Yk7owGAcWjwMVRwrTesJEwB7WVOiILLI | | ``same as above``<br>``(echo I am user bandit23 \| md5sum \| cut -d ' ' -f 1)``<br>``cat /tmp/<tmp_new_dir> ``|
| level23 | jc1udXuA1tiHqjIsL8yaapX5XIAI6i0n | | ``mkdir /tmp/<name>``<br>``chmod 777 /tmp/<name>, cat -e "#!/bin/bash \ncat /etc/bandit_pass/bandit24 > /tmp/<name>/pass" > job24.sh``<br>``cp job24.sh /var/spool/bandit24/ ``|
| level24 | UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ | | ``seq -f "UoMYTrfrBFHyQXmg6gzctqAwOmw1IohZ %04g" 0000 9999 \| nc localhost 30002 ``|
| level25 | uNG9O58gUE7snukf3bvZ0rxhtnjzSGzG | | ``ls``<br>``(sshkey for l26) (dec the size of terminal before login to l26) ``|
| level26 | 5czgV9L3Xx8JPOyRbXh6lQbmIOWvPT6Z | | ``press v``<br>``type :set shell=/bin/bash``<br>``:shell, cat /etc/bandit_pass/bandit26``<br>``./bandit27-do cat /etc/bandit_pass/bandit27 ``|
| level27 | 3ba3118a22e93127a4ed485be72ef5ea | | ``cd /tmp/``<br>``git clone ssh://bandit27-git@localhost/home/bandit27-git/repo``<br>``cat repo/README`` |
| level28 | 0ef186ac70e04ea33b4c1853d2526fa2 | | ``cd /tmp/``<br>``git clone ssh://bandit28-git@localhost/home/bandit28-git/repo``<br>``git log``<br>``git log -p`` |
| level29 | bbc96594b4e001778eee9975372716b2 | | ``cd /tmp/``<br>``git clone ssh://bandit29-git@localhost/home/bandit29-git/repo``<br>``git branch -a``<br>``git checkout dev``<br>``cat README`` |
| level30 | 5b90576bedb2cc04c86a9e924ce42faf | | ``cd /tmp/``<br>`` git clone ssh://bandit30-git@localhost/home/bandit30-git/repo``<>br``git tag``<br>``git show <tah_name>`` |
| level31 | 47e603bb428404d265f59c42920d81e5 | | ``cd /tmp/, git clone ssh://bandit31-git@localhost/home/bandit31-git/repo, echo 'May I come in?' >key.txt``<br>``git add key.txt``<br>``rm .gitignore``<br> ``git commit -m 'key31'``<br>`` git push`` |
| level32 | 56a9bf19c63d650ce78e6ec0354ee45e | | ``$0``<br>``/bin/bash``<br>``cat /etc/bandit_pass/bandit33 ``|
| level33 | c9c3199ddf4121b10cf581a98d51caee | | ``--FINISH ``|
