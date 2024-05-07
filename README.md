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

## 2.2. Modifying the websocket port
When we try to run the client after the port for the client **only**, this happens:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/bd430744-b753-4663-b05e-800da6687e9d)

To make sure it runs properly, we need to change the port for the server side as well. Here is the part that we need to modify:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/3248e3e5-0648-469b-ad1b-f7024f48cfb5)
After changing the port from 2000 to  8080, we can then finally run the client successfully:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/e53675c6-368d-4cdc-a921-c3f6c67c6e86)

## 2.3 Small changes. Add some information to client
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/2b47f93c-4e9a-4570-b7e3-f7962583744f)
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/c5a1ba3e-c371-47be-a691-7bbf3f21a20b)
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/8faf76d1-4e1b-41ae-b1d3-8cea630c2a71)

Theres a small change we can do to show a bit more information about where each message comes from. First, we do a little modification on the client code to show more information about who the sender is:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/43078088-94d2-4d92-aee2-25d11630c4d8)

And then, we change the server:
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/63010f7a-c339-4464-a6a2-27a4bca40a56)
![image](https://github.com/ternaksapi/modul10_tutorial2_chat/assets/116947973/dc0b4aeb-fc07-4f92-af9e-f89acdd9010f)

The change is so that everytime the server is going to broadcast the message, it is also going to include where the sender is from through `addr`
