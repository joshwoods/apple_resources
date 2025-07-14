

- App Store Connect API
-  Manually Release an App Store Approved Version of Your App 

Web Service Endpoint

# Manually Release an App Store Approved Version of Your App

Release an approved version of your app to the App Store.

App Store Connect API 1.5+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/appStoreVersionReleaseRequests
```

## HTTP Body

AppStoreVersionReleaseRequestCreateRequest

The request body you use to manually release an approved version of your app to the App Store.

Content-Type: application/json

## Response Codes

` 201 ``Created`

AppStoreVersionReleaseRequestResponse

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

## Discussion

When you submit your app for review, if itʼs approved and the status changes to Pending Developer Release, then you can release a version. For more information about app review, see Submit for review. For more information about manually releasing versions, see Select a version release option. For more information about app status, see App and submission statuses.

Important

Send this request only when you’re ready to publish your version. You can’t cancel this request.

