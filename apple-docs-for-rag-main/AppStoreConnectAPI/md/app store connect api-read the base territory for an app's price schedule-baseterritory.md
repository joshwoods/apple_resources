

- App Store Connect API
-  Read the base territory for an app's price schedule 

Web Service Endpoint

# Read the base territory for an app's price schedule

Read the base territory and currency for a specific app.

App Store Connect API 2.3+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appPriceSchedules/{id}/baseTerritory
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource. Obtain the app resource ID from the List Apps response.

## Query Parameters

`fields[territories]`

`[string]`

Value: `currency`

## Response Codes

` 200 ``OK`

TerritoryResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/baseTerritory
```

```
{
  "data" : {
    "type" : "territories",
    "id" : "CAN",
    "attributes" : {
      "currency" : "CAD"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/territories/CAN"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/appPriceSchedules/6447402192/baseTerritory"
  }
}
```

## See Also

### Getting and managing an app’s price schedules

Read price schedule information for an app

Read price schedule details for a specific app.

Read an app's price schedule information

List the price schedule details for a specific app.

List automatically generated prices for an app

List the automatically calculated prices for an app generated from a base territory.

List manually chosen prices for an app

List the prices you chose for a specific app.

Add a scheduled price change to an app

Create a scheduled price change for an app.

