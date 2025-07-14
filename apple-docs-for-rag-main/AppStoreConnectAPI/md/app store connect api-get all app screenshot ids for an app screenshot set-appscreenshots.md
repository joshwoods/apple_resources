

- App Store Connect API
-  Get All App Screenshot IDs for an App Screenshot Set 

Web Service Endpoint

# Get All App Screenshot IDs for an App Screenshot Set

Get the ordered screenshot IDs in a screenshot set.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appScreenshotSets/{id}/relationships/appScreenshots
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`limit`

`integer`

Maximum: `200`

## Response Codes

` 200 ``OK`

AppScreenshotSetAppScreenshotsLinkagesResponse

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

### Listing and Reordering All Screenshots in a Set

List All App Screenshots for an App Screenshot Set

List all ordered screenshots in a screenshot set.

Replace All App Screenshots for an App Screenshot Set

Change the order of the screenshots in a screenshot set.

