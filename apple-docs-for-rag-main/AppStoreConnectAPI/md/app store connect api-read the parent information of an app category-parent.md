

- App Store Connect API
-  Read the Parent Information of an App Category 

Web Service Endpoint

# Read the Parent Information of an App Category

Get the App Store category to which a specific subcategory belongs.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCategories/{id}/parent
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appCategories]`

`[string]`

Possible Values: `platforms, subcategories, parent`

## Response Codes

` 200 ``OK`

AppCategoryWithoutIncludesResponse

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

Read App Category Information

Get a specific app category.

