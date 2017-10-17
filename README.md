# Documentation

## Restaurant

### Property

* restaurant name `Both Chinese and English`
* icon
* menu images
* food images
* address
* postcode
* ~~~location `Geohash or PostGIS`~~~
* location `Google Place IDs`
* rating `1 to 5`
* contact `Phone Num`
* opening hours
* averange cost
* type

### Type

1. Malay
1. Indian
1. Chinese
1. Western
1. Japanese
1. Korean
1. Steamboat
1. Buffet
1. Pizza

>feel free to add more :D

### API

#### User

___

Url | HTTP | Function
--- | --- | ---
<http://tinyseek.com/api/user/> | POST |register & login

#### Get Restaurant Data

___

##### Description

* >get restaurant data from a city

##### Request Url (Example)

* <http://tinyseek.com/api/restaurants/>

##### Request Method

* `GET`

##### Params

Name | Type | Description
--- | --- | ---
code | int | postcode
location | string | googlePlaceIds

##### Json Example

```Json
{
    "status_code": 0,
    "details":"https://..",
    "data": [
        {
            "id": "1",
            "status": "0",
            "area": "kota damansara",
            "title": "jiwawa's bbq",
            "menu_urls": [
                {
                ...
                }
            ],
            ...
        },
    ]
}
```
