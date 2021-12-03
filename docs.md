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
    "token": "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MTNkMmRmZTZlMmYwMzAwMjhhMmEwYzYiLCJuYW1lIjoiQXJ2aW5kIERpeGl0IiwicGhvbmVOdW1iZXIiOjk3OTM0ODI2NzAsImlhdCI6MTYzNjM3MjMwNCwiZXhwIjoxNjM2Mzc5NTA0fQ.bAVQruhMI2hdksSc2DmBLl7QSifNmAh8s3qT5C7UCMM",
    "response": {
        "_id": "613d2dfe6e2f030028a2a0c6",
        "name": "Arvind Dixit",
        "phoneNumber": 9793482670,
        "email": "arvinddixit@gmail.com",
        "isPasswordUpdated": false
    }
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
    "message": "4 bookings found",
    "response": [
        {
            "isServiceProviderAssigned": true,
            "isJobDone": false,
            "isRequestedToCancelService": false,
            "rating": 0,
            "amountPaidByCustomer": 0,
            "_id": "61723e7e73cbf90050721718",
            "services": [
                {
                    "quantity": 1,
                    "createdAt": "2021-10-22T04:27:47.180Z",
                    "_id": "61723dc35b3343003a49b8c7",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613a1ad900c2e7005be3eaf0",
                    "serviceName": "All in one ",
                    "actualPrice": 1837,
                    "discountedPrice": 1378
                }
            ],
            "isCancelled": false,
            "isAdminCancelledService": false,
            "isAdminApprovedCancellationRequest": false,
            "bookingId": "Ft3mRs_3W",
            "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
            "customerId": "61717e7dd12cd80028408c33",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401",
                "phoneNumber": "9415332242",
                "zipcode": "201305",
                "city": "Gautam Buddha Nagar",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "02:30 PM  -  03:00 PM",
            "serviceDate": "2021-10-23",
            "finalPrice": 1383,
            "cartAmount": 1378,
            "coupon": {
                "id": "61717edc5d4272002fd5211a",
                "name": "PM11",
                "amount": 20
            },
            "extraCharge": {
                "type": "hygenicFee",
                "amount": 25
            },
            "timeOfBooking": "2021-10-22T04:30:54.743Z",
            "createdAt": "2021-10-22T04:30:54.743Z",
            "approvedAt": "2021-10-22T04:30:54.743Z",
            "__v": 0,
            "serviceProvider": {
                "isPhoneVerified": false,
                "isPasswordUpdated": false,
                "_id": "613d2dfe6e2f030028a2a0c6",
                "name": "Arvind Dixit",
                "email": "arvinddixit@gmail.com",
                "phoneNumber": 9793482670,
                "password": "$2a$05$BRI.UitJ.7sdZIqCfRy3p.K6FUukkkyoYEbFgbho7ZmSLcZcJ4nO6",
                "initialPassword": "arvind@servimate",
                "imgUrl": "",
                "cityName": "Jaipur",
                "cityId": "60ec422a71c75d0015dac0f6",
                "serviceCategoryId": "610e411c5ef67b004487c5d8",
                "serviceCategoryName": "Make-Up",
                "remark": "Good",
                "certificates": [],
                "createdAt": "2021-09-11T22:30:22.972Z",
                "__v": 0
            },
            "serviceProviderId": "613d2dfe6e2f030028a2a0c6",
            "serviceProviderName": "Arvind Dixit"
        },
        {
            "isServiceProviderAssigned": true,
            "isJobDone": false,
            "isRequestedToCancelService": false,
            "rating": 0,
            "amountPaidByCustomer": 0,
            "_id": "617ac4f39fd13f00452bb0b9",
            "services": [
                {
                    "quantity": 1,
                    "createdAt": "2021-10-27T11:40:55.534Z",
                    "_id": "61793ac76413a6003aa7345f",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613cdc1f896e500021025183",
                    "serviceName": "Honey Wax (Full Arms, Underarms & Legs) + Threading",
                    "actualPrice": 850,
                    "discountedPrice": 499
                },
                {
                    "quantity": 1,
                    "createdAt": "2021-10-27T11:39:11.743Z",
                    "_id": "61793a5f830bd1002fa471e0",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613a1ad900c2e7005be3eaf0",
                    "serviceName": "All in one ",
                    "actualPrice": 1837,
                    "discountedPrice": 1378
                }
            ],
            "isCancelled": false,
            "isAdminCancelledService": false,
            "isAdminApprovedCancellationRequest": false,
            "bookingId": "oi224eR_D",
            "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
            "customerId": "61717c3c0f6b30006aa1528c",
            "customerName": "Pksingh",
            "address": {
                "name": "pramod singh",
                "address": "sijua katras",
                "phoneNumber": "9060709987",
                "zipcode": 828121,
                "city": "Dhanbad",
                "state": "Jharkhand"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "01:30 PM  -  02:00 PM",
            "serviceDate": "2021-10-29",
            "finalPrice": 1902,
            "cartAmount": 1877,
            "extraCharge": {
                "type": "hygenicFee",
                "amount": 25
            },
            "timeOfBooking": "2021-10-28T15:42:43.568Z",
            "createdAt": "2021-10-28T15:42:43.568Z",
            "approvedAt": "2021-10-28T15:42:43.568Z",
            "__v": 0,
            "serviceProvider": {
                "_id": "613d2dfe6e2f030028a2a0c6",
                "name": "Arvind Dixit",
                "email": "arvinddixit@gmail.com",
                "phoneNumber": 9793482670,
                "imgUrl": ""
            },
            "serviceProviderId": "613d2dfe6e2f030028a2a0c6",
            "serviceProviderName": "Arvind Dixit"
        },
        {
            "isServiceProviderAssigned": true,
            "isJobDone": false,
            "isRequestedToCancelService": false,
            "rating": 0,
            "amountPaidByCustomer": 0,
            "_id": "617face4463b1400284f7c76",
            "services": [
                {
                    "quantity": 1,
                    "createdAt": "2021-11-01T09:00:10.955Z",
                    "_id": "617fac9ab84ff70066b8974c",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613cdc1f896e500021025183",
                    "serviceName": "Honey Wax (Full Arms, Underarms & Legs) + Threading",
                    "actualPrice": 850,
                    "discountedPrice": 499
                }
            ],
            "isCancelled": false,
            "isAdminCancelledService": false,
            "isAdminApprovedCancellationRequest": false,
            "bookingId": "4Wxxz5jbF",
            "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
            "customerId": "61794187830bd1002fa471e1",
            "customerName": "Rahul yadav",
            "address": {
                "name": "Kamal ",
                "address": "D5 3rd c ",
                "phoneNumber": "9571577784",
                "zipcode": "333504",
                "city": "Jhujhunu",
                "state": "Rajasthan"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "06:00 PM  -  06:30 PM",
            "serviceDate": "2021-11-01",
            "finalPrice": 524,
            "cartAmount": 499,
            "extraCharge": {
                "type": "hygenicFee",
                "amount": 25
            },
            "timeOfBooking": "2021-11-01T09:01:24.386Z",
            "createdAt": "2021-11-01T09:01:24.386Z",
            "approvedAt": "2021-11-01T09:01:24.386Z",
            "__v": 0,
            "serviceProvider": {
                "isPhoneVerified": false,
                "isPasswordUpdated": false,
                "_id": "613d2dfe6e2f030028a2a0c6",
                "name": "Arvind Dixit",
                "email": "arvinddixit@gmail.com",
                "phoneNumber": 9793482670,
                "password": "$2a$05$BRI.UitJ.7sdZIqCfRy3p.K6FUukkkyoYEbFgbho7ZmSLcZcJ4nO6",
                "initialPassword": "arvind@servimate",
                "imgUrl": "",
                "cityName": "Jaipur",
                "cityId": "60ec422a71c75d0015dac0f6",
                "serviceCategoryId": "610e411c5ef67b004487c5d8",
                "serviceCategoryName": "Make-Up",
                "remark": "Good",
                "certificates": [],
                "createdAt": "2021-09-11T22:30:22.972Z",
                "__v": 0
            },
            "serviceProviderId": "613d2dfe6e2f030028a2a0c6",
            "serviceProviderName": "Arvind Dixit"
        },
        {
            "isServiceProviderAssigned": true,
            "isJobDone": false,
            "isRequestedToCancelService": false,
            "rating": 0,
            "amountPaidByCustomer": 0,
            "_id": "617ff731b04c0c0050380982",
            "services": [
                {
                    "quantity": 1,
                    "createdAt": "2021-11-01T14:17:12.314Z",
                    "_id": "617ff6e8c486140021f99c38",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613a1ad900c2e7005be3eaf0",
                    "serviceName": "All in one ",
                    "actualPrice": 1837,
                    "discountedPrice": 1378
                }
            ],
            "isCancelled": false,
            "isAdminCancelledService": false,
            "isAdminApprovedCancellationRequest": false,
            "bookingId": "L-jeR09ZZ",
            "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
            "customerId": "61717c3c0f6b30006aa1528c",
            "customerName": "Pksingh",
            "address": {
                "name": "pramod singh",
                "address": "sijua katras",
                "phoneNumber": "9060709987",
                "zipcode": 828121,
                "city": "Dhanbad",
                "state": "Jharkhand"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "01:00 PM  -  01:30 PM",
            "serviceDate": "2021-11-16",
            "finalPrice": 1403,
            "cartAmount": 1378,
            "extraCharge": {
                "type": "hygenicFee",
                "amount": 25
            },
            "timeOfBooking": "2021-11-01T14:18:25.383Z",
            "createdAt": "2021-11-01T14:18:25.383Z",
            "approvedAt": "2021-11-01T14:18:25.384Z",
            "__v": 0,
            "serviceProvider": {
                "isPhoneVerified": false,
                "zipcodes": [],
                "isPasswordUpdated": true,
                "_id": "613d2dfe6e2f030028a2a0c6",
                "name": "Arvind Dixit",
                "email": "arvinddixit@gmail.com",
                "phoneNumber": 9793482670,
                "password": "$2a$05$BRI.UitJ.7sdZIqCfRy3p.K6FUukkkyoYEbFgbho7ZmSLcZcJ4nO6",
                "initialPassword": "arvind@servimate",
                "imgUrl": "",
                "cityName": "Jaipur",
                "cityId": "60ec422a71c75d0015dac0f6",
                "serviceCategoryId": "610e411c5ef67b004487c5d8",
                "serviceCategoryName": "Make-Up",
                "remark": "Good",
                "certificates": [],
                "createdAt": "2021-09-11T22:30:22.972Z",
                "__v": 0,
                "newPassword": "$2a$05$rzYGSD1yGq1j14UJAF3JzeID5.iDGdjIHPU5N.DDBUiXOQb0tkas."
            },
            "serviceProviderId": "613d2dfe6e2f030028a2a0c6",
            "serviceProviderName": "Arvind Dixit"
        }
    ]
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

==============================================================================================================
**UPDATE PASSWORD**

**URL** : `/partner/dev/api/v1/updatePassword`
**Method** : `PUT`
**Header** : `application/json`
**Headers** : `Authorization` : `${token}`
**Auth required** : YES
**Permissions required** : None
## Request Body 

```json
{
    "oldPassword":"arvind@servimate",
    "newPassword":"arvinds@servimate"
}
```
## Success Response 
**Code** : `200`
**Response**
```json
{
    "success": true,
    "message": "Password updated successfully"
}
```

==============================================================================================================
**COMPLETE JOB**

**URL** : `/partner/dev/api/v1/completeJob`
**Method** : `POST`
**Header** : `application/json`
**Headers** : `Authorization` : `${token}`
**Auth required** : YES
**Permissions required** : None
## Request Body 

```json
{
    "bookingId":"617ac4f39fd13f00452bb0b9",
    "isPaid":true,
    "amountPaidByCustomer":400,
    "partnerFeedback":"He was good"
}
```
## Success Response 
**Code** : `200`
**Response**
```json
{
    "success": true,
    "message": "Job completed successfully",
    "response": {
        "isServiceProviderAssigned": true,
        "isJobDone": true,
        "isRequestedToCancelService": false,
        "rating": 0,
        "amountPaidByCustomer": 400,
        "_id": "617ac4f39fd13f00452bb0b9",
        "services": [
            {
                "quantity": 1,
                "createdAt": "2021-10-27T11:40:55.534Z",
                "_id": "61793ac76413a6003aa7345f",
                "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                "serviceId": "613cdc1f896e500021025183",
                "serviceName": "Honey Wax (Full Arms, Underarms & Legs) + Threading",
                "actualPrice": 850,
                "discountedPrice": 499
            },
            {
                "quantity": 1,
                "createdAt": "2021-10-27T11:39:11.743Z",
                "_id": "61793a5f830bd1002fa471e0",
                "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                "serviceId": "613a1ad900c2e7005be3eaf0",
                "serviceName": "All in one ",
                "actualPrice": 1837,
                "discountedPrice": 1378
            }
        ],
        "isCancelled": false,
        "isAdminCancelledService": false,
        "isAdminApprovedCancellationRequest": false,
        "bookingId": "oi224eR_D",
        "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
        "customerId": "61717c3c0f6b30006aa1528c",
        "customerName": "Pksingh",
        "address": {
            "name": "pramod singh",
            "address": "sijua katras",
            "phoneNumber": "9060709987",
            "zipcode": 828121,
            "city": "Dhanbad",
            "state": "Jharkhand"
        },
        "modeOfPayment": "COD",
        "isPaid": true,
        "timeSlot": "01:30 PM  -  02:00 PM",
        "serviceDate": "2021-10-29",
        "finalPrice": 1902,
        "cartAmount": 1877,
        "extraCharge": {
            "type": "hygenicFee",
            "amount": 25
        },
        "timeOfBooking": "2021-10-28T15:42:43.568Z",
        "createdAt": "2021-10-28T15:42:43.568Z",
        "approvedAt": "2021-10-28T15:42:43.568Z",
        "__v": 0,
        "serviceProvider": {
            "_id": "613d2dfe6e2f030028a2a0c6",
            "name": "Arvind Dixit",
            "email": "arvinddixit@gmail.com",
            "phoneNumber": 9793482670,
            "imgUrl": ""
        },
        "serviceProviderId": "613d2dfe6e2f030028a2a0c6",
        "serviceProviderName": "Arvind Dixit"
    }
}
```
==============================================================================================================
**REQUESTED JOB**

**URL** : `/partner/dev/api/v1/bookings/requested`
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
    "count": 1,
    "message": "Here is the booking request",
    "response": [
        {
            "extraCharge": {
                "type": "hygenic",
                "amount": 25
            },
            "bookingJourney": {
                "isStarted": false,
                "isStopped": false,
                "isCustomerPaid": false,
                "amountPaidByCustomer": 0
            },
            "services": [
                {
                    "quantity": 1,
                    "createdAt": "2021-11-22T18:17:28.628Z",
                    "_id": "619bdeb8af020900629940f5",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613cdde3744f2d0062a6de5b",
                    "serviceName": "Fruit Facial",
                    "actualPrice": 657,
                    "discountedPrice": 450
                },
                {
                    "quantity": 1,
                    "createdAt": "2021-11-22T18:17:22.284Z",
                    "_id": "619bdeb20f1790005737de97",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613cdc9616be6600571fb647",
                    "serviceName": "Rica Waxology (Full arms, Legs & UA)",
                    "actualPrice": 1299,
                    "discountedPrice": 850
                },
                {
                    "quantity": 1,
                    "createdAt": "2021-11-22T18:17:19.885Z",
                    "_id": "619bdeafd4f824003af2c6c5",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613cdc1f896e500021025183",
                    "serviceName": "Honey Wax (Full Arms, Underarms & Legs) + Threading",
                    "actualPrice": 850,
                    "discountedPrice": 499
                },
                {
                    "quantity": 1,
                    "createdAt": "2021-11-22T18:17:10.041Z",
                    "_id": "619bdea6b5c4320028e5f40b",
                    "serviceCategory": "610bbcb4d5a9ca0039f4f1d0",
                    "serviceId": "613a1ad900c2e7005be3eaf0",
                    "serviceName": "All in one ",
                    "actualPrice": 1837,
                    "discountedPrice": 1378
                }
            ],
            "isServiceProviderAssigned": false,
            "isJobDone": false,
            "isRequestedToCancelService": false,
            "rating": 0,
            "isCancelled": false,
            "isAdminCancelledService": false,
            "isAdminApprovedCancellationRequest": false,
            "requestedServiceProviders": [
                "619140d1ddfb25430cb2e3fd",
                "619140f0ddfb25430cb2e3fe"
            ],
            "systemOrManual": 0,
            "isFeedbackGivenByCustomer": false,
            "_id": "619be06546f2c84f5071a4e8",
            "bookingId": "81lMez1A4",
            "serviceCategoryId": "610bbcb4d5a9ca0039f4f1d0",
            "customerId": "6191382c5142700050adac7e",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "cod",
            "isPaid": false,
            "timeSlot": "02:30 PM  -  03:00 PM",
            "serviceDate": "2021-11-28",
            "finalPrice": 3202,
            "cartAmount": 3177,
            "timeOfBooking": "2021-11-22T18:24:37.049Z",
            "createdAt": "2021-11-22T18:24:37.049Z",
            "approvedAt": "2021-11-22T18:24:37.049Z",
            "__v": 0
        }
    ]
}
```

==============================================================================================================
**ACCEPT JOB**

**URL** : `/partner/dev/api/v1/booking/accept/6191419c4250d65fe46e7c5d`
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
    "message": "Booking accepted successfully",
    "response": {
        "_id": "6191419c4250d65fe46e7c5d",
        "bookingId": "bHNHgea9A",
        "serviceProviderId": "619140d1ddfb25430cb2e3fd",
        "serviceProviderName": "Deepak Singh",
        "requestedServiceProviders": [],
        "isServiceProviderAssigned": true
    }
}
```

==============================================================================================================
**START JOB**

**URL** : `/partner/dev/api/v1/booking/start/6191419c4250d65fe46e7c5d`
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
    "message": "Job started successfully",
    "response": {
        "_id": "6191419c4250d65fe46e7c5d",
        "bookingId": "bHNHgea9A",
        "bookingJourney": {
            "stoppedAt": {},
            "isStarted": true,
            "isStopped": false,
            "isCustomerPaid": false,
            "amountPaidByCustomer": 0,
            "startedAt": "2021-11-22T18:38:46.936Z"
        }
    }
}
```

=============================================================================================================
**GET HOME SCREEN BANNER**

**URL** : `partner/dev/api/v1/homescreen/banner`
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
    "message": "1 banners found successfully",
    "response": [
        {
            "_id": "61a660dcbdc5ed4668b539a1",
            "title": "Banner 1",
            "picture": "https://res.cloudinary.com/dbzifmbj3/image/upload/v1638293725/pf3nwbo4dinsmotiaaxr.png",
            "createdAt": "2021-11-30T17:35:24.888Z",
            "__v": 0
        }
    ]
}
```

=============================================================================================================
**GET ALL COMPLETE BOOKINGS**

**URL** : `partner/dev/api/v1/bookings/completed`
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
    "count": 10,
    "message": "Here is the completed bookings",
    "response": [
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 400,
                "startedAt": "2021-11-22T18:38:46.936Z",
                "partnerFeedback": "He was good"
            },
            "isJobDone": true,
            "_id": "6191419c4250d65fe46e7c5d",
            "bookingId": "bHNHgea9A",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "cod",
            "isPaid": false,
            "timeSlot": "02:30 PM  -  03:00 PM",
            "serviceDate": "2021-11-28",
            "finalPrice": 1403,
            "timeOfBooking": "2021-11-14T17:04:28.324Z",
            "createdAt": "2021-11-14T17:04:28.324Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 5000,
                "startedAt": "2021-12-02T05:16:34.267Z"
            },
            "isJobDone": true,
            "_id": "619be06546f2c84f5071a4e8",
            "bookingId": "81lMez1A4",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "cod",
            "isPaid": false,
            "timeSlot": "02:30 PM  -  03:00 PM",
            "serviceDate": "2021-11-28",
            "finalPrice": 3202,
            "timeOfBooking": "2021-11-22T18:24:37.049Z",
            "createdAt": "2021-11-22T18:24:37.049Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 400,
                "startedAt": "2021-12-02T05:17:01.757Z"
            },
            "isJobDone": true,
            "_id": "619fab560f3e100021e60283",
            "bookingId": "mSIrp4b8s",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "03:30 PM  -  04:00 PM",
            "serviceDate": "2021-11-27",
            "finalPrice": 1403,
            "timeOfBooking": "2021-11-25T15:27:18.343Z",
            "createdAt": "2021-11-25T15:27:18.343Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 300,
                "startedAt": "2021-12-02T05:20:42.839Z"
            },
            "isJobDone": true,
            "_id": "619fb0c19fa9ab00508c1d7f",
            "bookingId": "9rFgTXiru",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "03:00 PM  -  03:30 PM",
            "serviceDate": "2021-11-28",
            "finalPrice": 1374,
            "timeOfBooking": "2021-11-25T15:50:25.641Z",
            "createdAt": "2021-11-25T15:50:25.641Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 80,
                "startedAt": "2021-12-02T05:22:27.868Z"
            },
            "isJobDone": true,
            "_id": "619fb51b4829360066038077",
            "bookingId": "lDfAnPZZu",
            "customerName": "Nishant Kumar",
            "address": {
                "name": "Nishant",
                "address": "Momo",
                "phoneNumber": "+917254844368",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "cod",
            "isPaid": false,
            "timeSlot": "02:30 PM  -  03:00 PM",
            "serviceDate": "2021-12-02",
            "finalPrice": 1403,
            "timeOfBooking": "2021-11-25T16:08:59.724Z",
            "createdAt": "2021-11-25T16:08:59.724Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 600,
                "startedAt": "2021-12-02T06:10:41.582Z"
            },
            "isJobDone": true,
            "_id": "619fb6a14829360066038079",
            "bookingId": "xIz5MdY7z",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "09:30 AM  -  10:30 AM",
            "serviceDate": "2021-11-27",
            "finalPrice": 1403,
            "timeOfBooking": "2021-11-25T16:15:29.963Z",
            "createdAt": "2021-11-25T16:15:29.963Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 330,
                "startedAt": "2021-12-02T06:12:01.602Z"
            },
            "isJobDone": true,
            "_id": "61a12b64b1cdab002ffbbc54",
            "bookingId": "lDyDWhTWK",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "03:00 PM  -  03:30 PM",
            "serviceDate": "2021-11-28",
            "finalPrice": 1403,
            "timeOfBooking": "2021-11-26T18:45:56.732Z",
            "createdAt": "2021-11-26T18:45:56.732Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": false,
                "amountPaidByCustomer": 40,
                "startedAt": "2021-12-02T13:57:35.491Z"
            },
            "isJobDone": true,
            "_id": "61a12bbe2d3fde003aeb1155",
            "bookingId": "KjPp_4V22",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "06:30 PM  -  07:00 PM",
            "serviceDate": "2021-11-30",
            "finalPrice": 1403,
            "timeOfBooking": "2021-11-26T18:47:26.113Z",
            "createdAt": "2021-11-26T18:47:26.113Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": false,
                "amountPaidByCustomer": 500,
                "startedAt": "2021-12-02T16:33:57.124Z"
            },
            "isJobDone": true,
            "_id": "61a58a8ab0ad090069e53d89",
            "bookingId": "YWWp5Wwu7",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak Singh",
                "address": "Tower A, 401, Supertech Ecociti",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "11:30 AM  -  12:00 PM",
            "serviceDate": "2021-12-01",
            "finalPrice": 4159,
            "timeOfBooking": "2021-11-30T02:20:58.909Z",
            "createdAt": "2021-11-30T02:20:58.909Z",
            "serviceProviderName": "Deepak Singh"
        },
        {
            "bookingJourney": {
                "isStarted": true,
                "isStopped": true,
                "isCustomerPaid": true,
                "amountPaidByCustomer": 600,
                "startedAt": "2021-12-02T06:15:22.653Z"
            },
            "isJobDone": true,
            "_id": "61a8644359009400457214a7",
            "bookingId": "8HEpRRmdV",
            "customerName": "Deepak Singh",
            "address": {
                "name": "Deepak",
                "address": "Momo",
                "phoneNumber": "+919415332242",
                "zipcode": 342311,
                "city": "Jodhpur",
                "state": "Uttar Pradesh"
            },
            "modeOfPayment": "COD",
            "isPaid": false,
            "timeSlot": "09:30 AM  -  10:30 AM",
            "serviceDate": "2021-12-01",
            "finalPrice": 580,
            "timeOfBooking": "2021-12-02T06:14:27.274Z",
            "createdAt": "2021-12-02T06:14:27.274Z",
            "serviceProviderName": "Deepak Singh"
        }
    ]
}
```