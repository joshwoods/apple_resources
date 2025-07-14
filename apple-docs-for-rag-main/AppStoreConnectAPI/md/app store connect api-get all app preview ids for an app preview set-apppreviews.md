

- App Store Connect API
-  Get All App Preview IDs for an App Preview Set 

Web Service Endpoint

# Get All App Preview IDs for an App Preview Set

Get the ordered app preview IDs in a preview set.

App Store Connect API 1.2+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appPreviewSets/{id}/relationships/appPreviews
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

AppPreviewSetAppPreviewsLinkagesResponse

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

### Listing and Reordering All Previews in a Set

List All App Previews for an App Preview Set

List all ordered app previews in a preview set.

Replace All App Previews for an App Preview Set

Change the order of the app previews in a preview set.

