# [Writeup] VolgaCTF 2021 Qualifier — Online Wallet (part 1) (Web 129 pt) 
Withdraw money from your account

This is an online wallet. There is a function to create and transfer funds between accounts.
To be flagged, more than 150 or negative funds must be withdrawn from the account.

![image](https://user-images.githubusercontent.com/81301788/112891885-dd147680-9102-11eb-8027-04b5b46a1753.png)

1 create wallet

![image](https://user-images.githubusercontent.com/81301788/112892183-341a4b80-9103-11eb-8ab0-ea6b5eb8f0ff.png)


2 Transfer token from Default Wallet to lnwza 99.98789745489548949849848974849841889494984984848498498419849849849484849494949849498494984985415418694865941895641851861896194189548941894198418941841984984984948484949494984949849498498541541869486594189564185186189619418954894189419841894184

![image](https://user-images.githubusercontent.com/81301788/112892008-0208e980-9103-11eb-8d81-f8ada57fe581.png)

3 Transfer from Default wallet to another 0.012102545104525575

![image](https://user-images.githubusercontent.com/81301788/112892284-544a0a80-9103-11eb-86d7-2f33df080311.png)

4 press withdraw

![image](https://user-images.githubusercontent.com/81301788/112892438-82c7e580-9103-11eb-95dc-eb71c2ae5d9e.png)

VolgaCTF{3723759ca308887d334afe8074ec9c23}

Node JSON.parse(‘{“amount”:100000000000000000000000000000000000000000000000000000000000001E-60}’).amount 100 MySQL select json_extract(‘{“amount”:100000000000000000000000000000000000000000000000000000000000001E-60}’, ‘$.amount’); 100.00000000000001

Due to different roundings in parsing, it was possible to take the balance into minus (Round-off error)

![image](https://user-images.githubusercontent.com/81301788/112892534-a0954a80-9103-11eb-8898-0590318b67c8.png)



