# Tutorial Modul 10 - Asynchronous Chat
---
### Muhammad Yusuf Haikal
### 2206081490
### Pemrograman Lanjut A
---

## 2.1. Original code of broadcast chat
Capture of the server:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/388f0b52-d4a5-45f8-8b8c-950b62a7fea2)

Capture of first client:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/380f5c52-f996-4064-b368-7accd5baf037)

Capture of second client:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/0a757cfb-4917-43e8-8e68-ad287ee54458)

Capture of third client:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/b3ef036c-c08e-47e6-8e83-bacd8de00731)

From the captures, we can observe how the app works. On the server side, we can see everytime a client sends a message, along with the adress and port where the message came from. It also shows everytime a new client connects to the server. Meanwhile on the client side, each client can send a message to the server and then the server broadcasts the message to every client thats connected.

