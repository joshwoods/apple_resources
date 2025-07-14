

- App Store Connect API
-  Modify App Store Review Details for an App Clip 

Web Service Endpoint

# Modify App Store Review Details for an App Clip

Update App Clip metadata you provide to App Store Review.

App Store Connect API 1.6+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/appClipAppStoreReviewDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Store Versions resource.

## HTTP Body

AppClipAppStoreReviewDetailUpdateRequest

The request body you use to update the App Store review details of an App Clip.

Content-Type: application/json

## Response Codes

` 200 ``OK`

AppClipAppStoreReviewDetailResponse

`OK`

The request completed successfully.

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

The provided resource data is not valid.

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## See Also

### Managing App Review Details for Your App Clip

Read the App Store Review Details of an App Clip

Get App Store Review details for an App Clip.

Create App Store Review Details for an App Clip

Provide App Clip metadata required by App Store Review.

