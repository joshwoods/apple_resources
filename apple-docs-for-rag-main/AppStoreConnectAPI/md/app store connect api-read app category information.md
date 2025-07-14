

- App Store Connect API
-  Read App Category Information 

Web Service Endpoint

# Read App Category Information

Get a specific app category.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCategories/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appCategories]`

`[string]`

Possible Values: `platforms, subcategories, parent`

`include`

`[string]`

Possible Values: `subcategories, parent`

`limit[subcategories]`

`integer`

Maximum: `50`

## Response Codes

` 200 ``OK`

AppCategoryResponse

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

` 404 ``Not Found`

ErrorResponse

`Not Found`

Resource not found.

Content-Type: application/json

## See Also

### Reading App Category Information

Read the Parent Information of an App Category

Get the App Store category to which a specific subcategory belongs.

