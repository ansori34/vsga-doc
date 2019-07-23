---
title: API Reference

toc_footers:
  - <a href='https://www.linkedin.com/in/rahmat-ansori/' target='_blank'>About Author</a>

includes:
  - errors
---

# Introduction

Welcome to the Item API! You can use our API to access Item API endpoints, which can get information on various items in our database.

# Items

## Get All Items

> The above command returns JSON structured like this:

```json
{
  "code": 200,
  "message": "Getting Items Success",
  "items": [
    {
      "id": 1,
      "brand": "MSI",
      "name": "MSI GL63 8RD Gaming Laptop",
      "price": 4000000
    },
    {
      "id": 2,
      "brand": "ASUS",
      "name": "ROG Strix XG32VQR Monitor",
      "price": 1000000
    }
  ]
}
```

This endpoint retrieves all items.

### HTTP Request

`GET https://vsga.herokuapp.com/<token>/item`

### URL Parameters

Parameter | Description
--------- | -----------
token | Create your own tokens to differentiate data from other participants

## Get a Specific Item

> The above command returns JSON structured like this:

```json
{
  "code": 200,
  "message": "Getting Item Success",
  "item": {
    "id": 1,
    "brand": "MSI",
    "name": "MSI GL63 8RD Gaming Laptop",
    "price": 4000000
  }
}
```

This endpoint retrieves a specific item.

### HTTP Request

`GET https://vsga.herokuapp.com/<token>/item/<id>`

### URL Parameters

Parameter | Description
--------- | -----------
token | Create your own tokens to differentiate data from other participants
id | The id of the item to retrieve

## Create an Item

> The above command returns JSON structured like this:

```json
{
  "code": 200,
  "message": "Adding Item Success"
}
```

This endpoint Create a new item.

### HTTP Request

`POST https://vsga.herokuapp.com/<token>/item/create`

### URL Parameters

Parameter | Method | Description
--------- | ------ | -----------
token | GET | Create your own tokens to differentiate data from other participants
name | POST | The new name for item
brand | POST | The new brand for item
price | POST | The new price for item

## Update a Specific Item

> The above command returns JSON structured like this:

```json
{
  "code": 200,
  "message": "Updating Item Success"
}
```

This endpoint update a specific item data.

### HTTP Request

`POST https://vsga.herokuapp.com/<token>/item/<id>/update`

### URL Parameters

Parameter | Method | Description
--------- | ------ | -----------
token | GET | Create your own tokens to differentiate data from other participants
id | GET | The id of the item to retrieve
name | POST | The new name for item
brand | POST | The new brand for item
price | POST | The new price for item

## Delete a Specific Item

> The above command returns JSON structured like this:

```json
{
  "code": 200,
  "message": "Deleting Item Success"
}
```

This endpoint deletes a specific item.

### HTTP Request

`GET https://vsga.herokuapp.com/<token>/item/<id>/delete`

### URL Parameters

Parameter | Description
--------- | -----------
token | Create your own tokens to differentiate data from other participants
id | The id of the item to retrieve