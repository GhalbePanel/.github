## Hi there 👋
### This is the **GhalbePanel**
A new panel has been created for you. if you are trying to make a server panel, for your gaming server, you can use the [GhalbePanel](#). its simple, and its eazy!
### Install
To install the panel, please go to the [GhalbePanel/Panel](https://github.com/ghalbepanel/panel) and click on the `Wiki` button to learn how to install the panel.
### How to use
To use the panel, you can simply after installation, set the panel server, but how?
1. Go to the panel directory
2. Go to the `Data` directory
3. Go to the `Server` directory
4. Open the `server.json` file
5. Here you can see the server basics, just put the port, the ip, the name, and the password.
6. Now you can start the server from the panel!
### How to make a server panel
Scince the panel is not supporting registering, you need to add accounts to the panel.

Simply make a api key and sent request to `/api/new` with the following data:

```json
{
    "username": "your username",
    "password": "your password",
    "email": "your email",
    "server_limit": -1, // -1 for unlimited, otherwise the limit of servers
    "admin": true // true for admin, false for normal user
}
```
then we need to sent the header `Authorization: Bearer <your api key>` to the panel.
### How to make changes?
To make changes to the panel, just open the directory, you need to know `PHP`, `HTML`, `CSS`, `JS` and `JSON`. then you can simply edit the panel.
### How to make discord bot for the panel?
You can simply use api to make discord bot for your panel, like hosting services in discord. but, if you don't know it, here is a example for you:
    
```py
import requests
import json
    
# to make a account
def make_account(username, password, email, server_limit, admin):
    data = {
        "username": username,
        "password": password,         "email": email,
        "server_limit": server_limit,
        "admin": admin
    }
    r = requests.post("https://panel.ghalbepanel.com/api/new", json=data)
    return r.json()
```
### Contribute
If you want to contribute to the panel, you can make a pull request on the [GhalbePanel/Panel](#).
### License
The panel is licensed under the [MIT license](#).
<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
