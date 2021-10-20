==============================================================================================================
**PARTNER LOGIN**

**URL** : `/partner/dev/api/v1/login`
**Method** : `POST`
**Header** : `application/json`
**Auth required** : None
**Permissions required** : None
## Request Body 
```json
{
    "phoneNumber":9793482670,
    "password":"arvind@servimate"
}
```
## Success Response 
**Code** : `200`
**Response**
```json
{
    "success": true,
    "message": "Logged in successfully",
    "token": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MTNkMmRmZTZlMmYwMzAwMjhhMmEwYzYiLCJuYW1lIjoiQXJ2aW5kIERpeGl0IiwicGhvbmVOdW1iZXIiOjk3OTM0ODI2NzAsImlhdCI6MTYzMTM5OTY4OSwiZXhwIjoxNjMxNDA2ODg5fQ.z2XBvtqYzXiOoFhjJ9k-U0mUfWKapLy8MoBTENFuRgQ"
}
```

==============================================================================================================
**GET ALL BOOKINGS**

**URL** : `/partner/dev/api/v1/bookings`
**Method** : `GET`
**Header** : `application/json`
**Headers** : `Authorization` : `${token}`
**Auth required** : YES
**Permissions required** : None

## Success Response 
**Code** : `200`
**Response**
```json
{
    "success": true,
    "message": "0 bookings found",
    "response": []
}
```
=============================================================================================================
**REGISTRATION  REQUEST**

**URL** : `/partner/dev/api/v1/registration/request`
**Method** : `POST`
**Header** : `application/json`
**Auth required** : None
**Permissions required** : None
## Request Body 

```json
{
    "name":"Brij Kishor",
    "phoneNumber":7080363723,
    "services": ["Men Grooming", "Men Hair cut"],
    "city":{
        "id":"60ec422a71c75d0015dac0f6",
        "name":"Jaipur"
    },
    "email":"brijkishor@gmail.com",
    "experience":1
}
```
## Success Response 
**Code** : `201`
**Response**
```json
{
    "success": true,
    "message": "Regisration request submitted successfully",
    "response": {
        "services": [
            "Men Grooming",
            "Men Hair cut"
        ],
        "_id": "616fb752e770c23e60b41a3f",
        "name": "Brij Kishor",
        "phoneNumber": 7080363723,
        "city": {
            "id": "60ec422a71c75d0015dac0f6",
            "name": "Jaipur"
        },
        "email": "brijkishor@gmail.com",
        "experience": 1,
        "createdAt": "2021-10-20T06:29:38.496Z",
        "__v": 0
    }
}
```

==============================================================================================================
**GET ALL CITIES**

**URL** : `/partner/dev/api/v1/city`
**Method** : `GET`
**Header** : `application/json`
**Headers** : `Authorization` : `${token}`
**Auth required** : YES
**Permissions required** : None

## Success Response 
**Code** : `200`
**Response**
```json
{
    "success": true,
    "message": "Cities fetched successfully",
    "response": [
        {
            "_id": "60ec422a71c75d0015dac0f6",
            "name": "Jaipur",
            "state": "Rajasthan"
        },
        {
            "_id": "60ec433171c75d0015dac0f8",
            "name": "Noida",
            "state": "Uttar Pradesh"
        },
        {
            "_id": "60ec44c571c75d0015dac0f9",
            "name": "Gurgaon ",
            "state": "Haryana"
        },
        {
            "_id": "60ec453171c75d0015dac0fa",
            "name": "Jodhpur",
            "state": "Rajasthan"
        },
        {
            "_id": "614c94697ccd90002f2f86c8",
            "name": "Test",
            "state": "Test"
        }
    ]
}
```
