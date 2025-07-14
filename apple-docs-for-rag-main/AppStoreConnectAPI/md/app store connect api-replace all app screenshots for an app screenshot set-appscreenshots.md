

- App Store Connect API
-  Replace All App Screenshots for an App Screenshot Set 

Web Service Endpoint

# Replace All App Screenshots for an App Screenshot Set

Change the order of the screenshots in a screenshot set.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appScreenshotSets/{id}/relationships/appScreenshots
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppScreenshotSetAppScreenshotsLinkagesRequest

Content-Type: application/json

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Listing and Reordering All Screenshots in a Set

Get All App Screenshot IDs for an App Screenshot Set

Get the ordered screenshot IDs in a screenshot set.

List All App Screenshots for an App Screenshot Set

List all ordered screenshots in a screenshot set.

