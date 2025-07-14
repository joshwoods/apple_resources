

- App Store Connect API
-  List Territories 

Web Service Endpoint

# List Territories

List all territories where the App Store operates.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/territories
```

## Query Parameters

`fields[territories]`

`[string]`

Value: `currency`

`limit`

`integer`

Number of resources to return.

Maximum: `200`

## Response Codes

` 200 ``OK`

TerritoriesResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

An error occurred with your request.

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Request not authorized.

Content-Type: application/json

## See Also

### Getting Territories

List All Territories for an End User License Agreement

List all the App Store territories to which a specific custom app license agreement applies.

