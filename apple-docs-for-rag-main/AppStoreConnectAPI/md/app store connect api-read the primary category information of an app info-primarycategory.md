

- App Store Connect API
-  Read the Primary Category Information of an App Info 

Web Service Endpoint

# Read the Primary Category Information of an App Info

Get an app’s primary App Store category.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appInfos/{id}/primaryCategory
```

## Path Parameters

`id`

`string`

 (Required) 

An opaque resource ID that uniquely identifies the resource.

## Query Parameters

`fields[appCategories]`

`[string]`

Fields to return for included related types.

Possible Values: `platforms, subcategories, parent`

`limit[subcategories]`

`integer`

Maximum: `50`

`include`

`[string]`

Possible Values: `subcategories, parent`

## Response Codes

` 200 ``OK`

AppCategoryResponse

`OK`

Request succeeded.

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Reading Categories

Read the Secondary Category Information of an App Info

Get an app’s secondary App Store category.

