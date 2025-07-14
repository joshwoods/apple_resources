

- App Store Connect API
-  Create App Store Review Details for an App Clip 

Web Service Endpoint

# Create App Store Review Details for an App Clip

Provide App Clip metadata required by App Store Review.

App Store Connect API 1.6+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appClipAppStoreReviewDetails
```

## HTTP Body

AppClipAppStoreReviewDetailCreateRequest

The request body you use to create App Store detail information.

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppClipAppStoreReviewDetailResponse

`Created`

The request completed successfully and a new App Clip App Store Review Details resource has been created.

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

Modify App Store Review Details for an App Clip

Update App Clip metadata you provide to App Store Review.

