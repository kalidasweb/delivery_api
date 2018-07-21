# Task Creation

Task Creation Api.

**URL** : `/api/new_order/`

**Method** : `POST`

**Auth required** : Yes

**Headers required**:

 ```x-client-data: <client_token>```

 ```x-client-date: <Current_Time_String>```

```Authorization: <auth_token>```


**Data constraints**

```json
{
    "data": {
        "status": "Unallocated",
        "type": 0,
        "method": "Pickup",
        "picktime": "2018-08-18T09:15:00.000Z",
        "loc_lat": 9.921193599999999,
        "loc_lng": 78.11938229999998,
        "pickup_ladd": 13.0826802,
        "pickup_long": 80.27071840000008,
        "sent_ladd": 0,
        "sent_long": 0,
        "is_geo_fence": 1,
        "geo_fence_meter": "500",
        "pick_address": "Chennai, Tamil Nadu, India",
        "notes": "books",
        "order_id": "439483943",
        "cust_name": "Kalidass",
        "cust_phone": "+919524609638",
        "cust_email": "",
        "cust_address": "Madurai Main, Madurai, Tamil Nadu, India",
        "sender_number": "+919382923222",
        "schedule_date_time": "2018-09-07 14:45",
        "pick_date_time": "2018-08-18 14:45"
    },
    "cust_email": "",
    "sender_number": "+919382923222",
    "sent_ladd": 0,
    "sent_long": 0
}


```

**Data example**

```json
{
    "data": {
        "status": "Unallocated",
        "type": 0,
        "method": "Pickup",
        "picktime": "2018-08-18T09:15:00.000Z",
        "loc_lat": 9.921193599999999,
        "loc_lng": 78.11938229999998,
        "pickup_ladd": 13.0826802,
        "pickup_long": 80.27071840000008,
        "sent_ladd": 0,
        "sent_long": 0,
        "is_geo_fence": 1,
        "geo_fence_meter": "500",
        "pick_address": "Chennai, Tamil Nadu, India",
        "notes": "books",
        "order_id": "439483943",
        "cust_name": "Kalidass",
        "cust_phone": "+919524609638",
        "cust_email": "",
        "cust_address": "Madurai Main, Madurai, Tamil Nadu, India",
        "sender_number": "+919382923222",
        "schedule_date_time": "2018-09-07 14:45",
        "pick_date_time": "2018-08-18 14:45"
    },
    "cust_email": "",
    "sender_number": "+919382923222",
    "sent_ladd": 0,
    "sent_long": 0
}

```



## Success Response

**Code** : `200 OK`

**Content example**

```json

{
    "data": "Task Created",
    "status": "ok"
}


```

## Error Response

**Content** :

```json
{
    "data": "<Error Msg>",
    "status": "error"
}
```
