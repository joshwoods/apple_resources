

- App Store Connect API
-  List All Subcategories for an App Category 

Web Service Endpoint

# List All Subcategories for an App Category

List all App Store subcategories that belong to a specific category.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appCategories/{id}/subcategories
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[appCategories]`

`[string]`

Possible Values: `platforms, subcategories, parent`

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AppCategoriesWithoutIncludesResponse

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

### Listing Categories and Subcategories

List App Categories

List all categories on the App Store, including the category and subcategory hierarchy.

