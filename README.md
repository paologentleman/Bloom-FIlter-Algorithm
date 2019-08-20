# Personalized Bloom FIlter Algorithm
Personalized version of the Bloom Filter Algorithm for duplicate detection of massive datasets of passwords.

![alt text](https://miro.medium.com/max/1838/1*HKQtaB1_m6Bt7xqTKr-HXg.png)

## 2A) Find the ***duplicates***!

Given [`passwords2.txt`](https://drive.google.com/open?id=1wTmOU-yqk4qdQYg42AquhzgpNGrRA96d), a 2GB file of alphanumeric passwords as input, each row corresponds to a string of 20 characters. The goal is to check whether there are some duplicate strings. Our definition of duplicate is that the two strings have the __same characters__, order is not important. Thus, "AABA" = "AAAB".

* We know In the file there are 10M duplicates, can we detect them?
* Does it happen that two strings with different characters are hashed to the same value? If yes, could you provide the number of *False Positive*?

## 2B) Find the ***exact duplicates***
Now do the same thing as before, but now the order of the characters must be put into account. Example: "AABA" != "AAAB".
