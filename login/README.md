# Login

Used to collect a Token for a registered User.

**URL** : `/api/auth?api=web`

**Method** : `POST`

**Auth required** : NO

**Headers required**:

 ```x-client-data: <client_token>```


**Data constraints**

```json
{
    "data": {
        "email": "[valid email address]",
        "password": "[password in plain text]"
    }
}

```

**Data example**

```json
{
    "data": {
        "email": "[valid email address]",
        "password": "[password in plain text]"
    }
}
```

## Success Response

**Code** : `200 OK`

**Content example**

```json
{
    "data": {
        "token": "<auth_token>",
        "role": "manager",
        "gps_active": 1,
        "demo_links": null
    },
    "status": "ok"
}
```

## Error Response

**Condition** : If 'username' and 'password' combination is wrong.

**Content** :

```json
{
    "data": "<Error Msg>",
    "status": "error"
}
```
