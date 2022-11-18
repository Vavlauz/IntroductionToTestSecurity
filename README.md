# **Введение в тестирование безопасности**

**Ссылка на домашнее задание/требования:** https://github.com/netology-code/ibqa-homeworks/blob/main/1.%20Intro/homework_lecture1.md

## **Wireshark, UDP**

![UDP](/UDP.png)

Sourсe port: **55432**

Destanation port: **8995**

## **Wireshark, DNS**

![DNS1](/DNS.png)

![DNS2](/DNS2.png)


Флаги протокола DNS, которые удалось обнаружить:

- 0x0100 Standard query
- 0x8180 Standard query response, No error

  1... .... .... .... = Response: Message is a response

.000 0... .... .... = Opcode: Standard query (0)

.... .0.. .... .... = Authoritative: Server is not an authority for domain

.... ..0. .... .... = Truncated: Message is not truncated

.... ...1 .... .... = Recursion desired: Do query recursively

.... .... 1... .... = Recursion available: Server can do recursive queries

.... .... .0.. .... = Z: reserved (0)

.... .... ..0. .... = Answer authenticated: Answer/authority portion was not authenticated by the server

.... .... ...0 .... = Non-authenticated data: Unacceptable

.... .... .... 0000 = Reply code: No error (0)

## **ZAP**

![ID](/ID.png)