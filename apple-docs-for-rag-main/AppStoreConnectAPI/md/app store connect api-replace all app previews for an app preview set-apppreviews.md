

- App Store Connect API
-  Replace All App Previews for an App Preview Set 

Web Service Endpoint

# Replace All App Previews for an App Preview Set

Change the order of the app previews in a preview set.

App Store Connect API 1.2+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appPreviewSets/{id}/relationships/appPreviews
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

AppPreviewSetAppPreviewsLinkagesRequest

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

### Listing and Reordering All Previews in a Set

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

Get All App Preview IDs for an App Preview Set

Get the ordered app preview IDs in a preview set.

