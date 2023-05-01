Ход решения машины

1. nmap -sS -sV -O {IP}
Просканил жертву, увидели 139, 445 и 3389 порты открытыми


2. nmap -p 139,445 -Pn --script smb-vuln* {IP}
Просканировали nmap'ом на уязвимости SMB протокола, увидели, что уязвим MS08-67 и MS17-010

3. Применили эксплойт

4. Нашли флаг на рабочем столе



[Black], [red] - цвета цепочек решения для того или иного последовательности решения

Решение для MS08-67 - [black] https://eslam3kl.medium.com/hack-the-box-legacy-c245030172ae


Решение для MS17-010 - [red] https://ethicalhacs.com/legacy-hackthebox-walkthrough/
