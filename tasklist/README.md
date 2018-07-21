# Task List

Get all task belongs to your account.

**URL** : `/api/new_order/`

**Method** : `GET`

**Auth required** : Yes

**Headers required**:

 ```x-client-data: <client_token>```

 ```x-client-date: <Current_Time_String>```

```Authorization: <auth_token>```


## Success Response

**Code** : `200 OK`

**Content example**

```json

{
    "data": [{
        "id": 1157,
        "cust_id": 1266,
        "status": "Allocated",
        "type": "0",
        "notes": "",
        "created_at": "2018-07-21 08:56:53",
        "deleted_at": null,
        "updated_at": "2018-07-21 08:57:08",
        "lat": "",
        "lng": "",
        "delivery_to": null,
        "delivery_phone": null,
        "timestamps": null,
        "is_cust_delivery": 1,
        "remarks": null,
        "added_by": 46158,
        "cust_phone": "+919594949663",
        "signature": null,
        "schedule_date_time": "2018-07-21 23:25:00",
        "is_new_address": 1,
        "cust_address": "",
        "loc_lng": "-83.42058",
        "loc_lat": "42.495522",
        "method": "Pickup",
        "is_geo_fence": 1,
        "geo_fence_meter": 200,
        "delivery_time": null,
        "contact_person": null,
        "pickup_location": null,
        "order_id": "2345",
        "multidelivery": null,
        "multipickup": null,
        "pickup_long": "12.94996",
        "pickup_ladd": "80.237728",
        "picktime": "2018-07-21 15:10:00",
        "sender_name": null,
        "sender_number": "",
        "pick_address": "",
        "cust_email": null,
        "mob": null,
        "exact_delivery": null,
        "sent_address": null,
        "comments": null,
        "cust_name": "hmjhfhjf",
        "allocated_emp": "prince n",
        "allocated_emp_id": 46497,
        "cust": {
            "id": 1266,
            "name": "",
            "loc_lat": "42.495522",
            "loc_lng": "-83.42058",
            "address": ""
        }
    }],
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
