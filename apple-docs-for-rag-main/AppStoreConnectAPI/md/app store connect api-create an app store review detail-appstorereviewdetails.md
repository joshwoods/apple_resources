

- App Store Connect API
-  Create an App Store Review Detail 

Web Service Endpoint

# Create an App Store Review Detail

Add App Store review details to an App Store version, including contact and demo account information.

App Store Connect API 1.2+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreReviewDetails
```

## HTTP Body

AppStoreReviewDetailCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreReviewDetailResponse

`Created`

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

### Creating, Modifying, and Reading Review Details

Read App Store Review Detail Information

Get App Review details you provided, including contact information, demo account, and notes.

Modify an App Store Review Detail

Update the app store review details, including the contact information, demo account, and notes.

