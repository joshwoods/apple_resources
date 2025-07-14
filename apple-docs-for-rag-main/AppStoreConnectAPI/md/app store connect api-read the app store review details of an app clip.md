

- App Store Connect API
-  Read the App Store Review Details of an App Clip 

Web Service Endpoint

# Read the App Store Review Details of an App Clip

Get App Store Review details for an App Clip.

App Store Connect API 1.6+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/appClipAppStoreReviewDetails/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the App Clip App Store Review Details resource.

## Query Parameters

`fields[appClipAppStoreReviewDetails]`

`[string]`

Additional fields to include for each App Clip App Store Review Details resource returned by the response.

Possible Values: `invocationUrls, appClipDefaultExperience`

`include`

`[string]`

The relationship data to include in the response.

Value: `appClipDefaultExperience`

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

## See Also

### Managing App Review Details for Your App Clip

Create App Store Review Details for an App Clip

Provide App Clip metadata required by App Store Review.

Modify App Store Review Details for an App Clip

Update App Clip metadata you provide to App Store Review.

