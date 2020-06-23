# 3NAME FAQ

## How to code a sniper

First off, you will need:

 * Coding knowledge
 * A way to send HTTP requests
 * Knowledge with how HTTP works

### Requests

#### General info

All of these requests use a bearer token from the site. Bearer tokens have a max life of 2 hours. You may try to use [this](https://wiki.vg/Authentication#Refresh) to keep them alive for longer, but I haven't had any success.

Information sourced from (here)[https://wiki.vg/Mojang_API].

All of the requests below go to `https://api.mojang.com`.

#### Setting a name
```
POST api.mojang.com/user/profile/<uuid>/name
Authorization: Bearer <token>
Content-Type: application/json


{'name': '<name>', 'password': 'password'}
```

#### Blocking a name
```
PUT /user/profile/agent/minecraft/name/<name>
Authorization: Bearer <token>
Content-Length: 0


```

[Back to Home](index.html)
*3NAME rights belong to [Jamsheed Mistri](http://jmistri.com), this is only a site for common questions.*
