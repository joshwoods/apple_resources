

- App Store Connect API
-  Read the Primary Subcategory One Information of an App Info 

Web Service Endpoint

# Read the Primary Subcategory One Information of an App Info

Get the first App Store subcategory within an app’s primary category.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appInfos/{id}/primarySubcategoryOne
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

### Reading Subcategories

Read the Primary Subcategory Two Information of an App Info

Get the second App Store subcategory within an app’s primary category.

Read the Secondary Subcategory One Information of an App Info

Get the first App Store subcategory within an app’s secondary category.

Read the Secondary Subcategory Two Information of an App Info

Get the second App Store subcategory within an app’s secondary category.

