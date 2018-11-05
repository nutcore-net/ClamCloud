## default return

```json
{
    "result": "success",
    "data": {}
}
```

## system conf

### global
```json
{
    "admin":[...]
}
```

### threads-conf
```json
{
    "admin":[...],
    "report_max":\[0-9]+\,
    "method":["wl","bl","allow"]//whitelist/blacklist
}
```

### votes-conf
```json
{
    "admin":[...],
    "method":["wl","bl","allow"]//whitelist/blacklist
}
```

### users-conf
```json
{
    "admin":[...],
    "email_verify":[true,false],
    "email_conf":
    {
        "server":"",
        "port":[1,65535],
        "user":"",
        "pswd":""
    },
    "useOAuth":[true,false],
    "OAuth":
    [
        {
            "state":"",
            "appkey":"",
            "appsecret":"",
            "uri":""
        },...
    ]
}
```

### events-conf
```json
{
    "admin":[...],
    "method":["wl","bl","allow"]//whitelist/blacklist
}
```

### groups-conf
```json
{
    "admin":[...],
    "method":["wl","bl","allow"]//whitelist/blacklist
}
```

### msgs-conf
```json
{
    "method":["wl","bl","allow"]//whitelist/blacklist
}
```

### attaches-conf
```json
{
    ""
    "method":["wl","bl","allow"]//whitelist/blacklist
}
```

## Info

### uInfo

```json
{
    "name":"",
    "bio":""
}
```

### uConf

```json
{
    "email":"",
    "email_valid":[true,false],
    "mute_msg":[true,false]
}
```

### vtInfo

```json
{
    "title":"",
    "body":"",
    "author":\[0-9]+\,//Not In Update(NIU)
    "options":
    [
        {
            "type":["vote","option"],
            "vtID":\[0-9]+\,
            "title":"",
            "sum":\[0-9]+\,
            "supports":[...]
        }
    ],
    "startTime":"",
    "endTime":""
}
```

### tdInfo

```json
{
    "title":"",
    "body":"",
    "author":\[0-9]+\,//NIU
    "reports":[...],//NIU
    "time":"",//NIU
    "writable":[...]//NIU
}
```

### gpInfo

```json
{
    "name":"",
    "bio":""
}
```

### gpConf

```json
{
    "admin":[...],
    "join":["open","apply","invite"],
    "allow_msg":[true/false],
}
```