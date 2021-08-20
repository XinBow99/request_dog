<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="./DemoPhotos/robot.png" alt="Project logo"></a>
</p>
<h3 align="center">POPDOG BOT</h3>

<div align="center">

[![Status](https://img.shields.io/badge/status-active-success.svg)]()
[![GitHub Issues](https://img.shields.io/github/issues/XinBow99/popdog_bot.svg)](https://github.com/XinBow99/popdog_bot/issues)
[![GitHub Pull Requests](https://img.shields.io/github/issues-pr/XinBow99/popdog_bot.svg)](https://github.com/XinBow99/popdog_bot/pulls)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](/LICENSE)

</div>

---

<p align="center"> POPDOG Bot is a Python application for auto request click event of popdog RESTApi.
    <br> 
</p>

---

## 📝 Table of Contents

- [Installation](#Installation)
- [About](#about)
- [Usage](#usage)
- [Demo figures](#Demofigures)

---

## Installation <a name = "Installation"></a>

Make sure your environment have those package.
- flask
- flask_cors
- threading
- requests
- time
- random
- argparse
- sys
- json

and `python version >= 3`

---

## About <a name = "about"></a>
### How to get uuid
Open the Developer Tools on your browser, and switch to `Application` tab.
![uuid](./DemoPhotos/uuid.png "uuid")
you can also insert `uuid`
![uuid2](./DemoPhotos/console.png "uuid2")
If you want get new uuid, call this route 
```
https://popdog.click/uuid
```
or clear Storage on browser and refresh.
---

## 🏁 Usage <a name = "usage"></a>
### If you `only have an public IP.`
#### Please run this bash command. 
If you `only have an IP` or you want start on `one server(computer)`.
```bash
$python3 BotStart_NoAnotherIP.py -p 8080 -t trigger
```
- `-p` is Server start port
- `-t` is Server trigger route

Now you can access these routes.

To create a bot event
- http://`<ip>`:`<port>`/`<trigger-value>`/create/`<Bot_Name>`/`<Bot_UUID>`

To visit bot status

- http://`<ip>`:`<port>`/`<trigger-value>`/lastupdate

#### Success figure of start.
![start_one_ip](./DemoPhotos/start_one_ip.png "start_one_ip")

---
### If you have more than the one public ip.
#### Please run this bash command. 
```bash
$python3 BotStart_HaveAnotherIP.py -p 18006 -t test_trigger -cip 172.18.18.18 -cp 18006 -ct test_trigger
```
- `-p` is Server start port
- `-t` is Server trigger route
- `-cip` is Another Server of public ip or domain
- `-cp` is Another Server of running port
- `-ct` is Another Server of running trigger route

Now you can access these routes.

To create a bot event
- http://`<ip>`:`<port>`/`<trigger-value>`/create/`<Bot_Name>`/`<Bot_UUID>`

To visit bot status

- http://`<ip>`:`<port>`/`<trigger-value>`/lastupdate

#### Success figure of start.
![start_another](./DemoPhotos/start_another.png "start_another")

---

## 🎈 Demo figures <a name="Demofigures"></a>

