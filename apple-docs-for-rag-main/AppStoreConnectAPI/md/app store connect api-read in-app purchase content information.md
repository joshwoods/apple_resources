

- App Store Connect API
-  Read In-App Purchase Content Information 

Web Service Endpoint

# Read In-App Purchase Content Information

Get details about uploaded in-app purchase content.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/inAppPurchaseContents/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[inAppPurchaseContents]`

`[string]`

Possible Values: `fileName, fileSize, url, lastModifiedDate, inAppPurchaseV2`

`include`

`[string]`

Value: `inAppPurchaseV2`

## Response Codes

` 200 ``OK`

InAppPurchaseContentResponse

`OK`

Content-Type: application/json

` 400 ``Bad Request`

ErrorResponse

`Bad Request`

Content-Type: application/json

` 401 ``Unauthorized`

ErrorResponse

`Unauthorized`

Content-Type: application/json

` 403 ``Forbidden`

ErrorResponse

`Forbidden`

Content-Type: application/json

` 404 ``Not Found`

ErrorResponse

`Not Found`

Content-Type: application/json

## See Also

### Endpoints

Create an In-App Purchase

Create an in-app purchase, including a consumable, non-consumable, or non-renewing subscription.

Read In-App Purchase Information

Get information about a specific in-app purchase.

List All In-App Purchases for an App

Get a list of the in-app purchases for a specific app.

Modify an In-App Purchase

Update the reference name of a specific in-app purchase.

Delete an In-App Purchase

Delete a specific in-app purchase from your app.

List All Price Points for an In-App Purchase

Get a list of possible price points for an in-app purchase.

List all in-app purchase price point equalizations

Get a list of in-app purchase price points and their equivalent in a specified currency.

Read Promoted Purchase Information for an In-App Purchase

Get details about the promoted purchase of an in-app purchase.

List All Localizations for an In-App Purchase

Get a list of localized display names and descriptions for a specific in-app purchase.

Read Review Screenshot Information for an In-App Purchase

Get information about a review screenshot for a specific in-app purchase.

Create a Review Submission for an In-App Purchase

Create an in-app purchase submission for review.

Read the Price Schedule for an In-App Purchase

Get a list of the scheduled prices for an in-app purchase.

Read Content Information for an In-App Purchase

Get the details about hosted content for an in-app purchase.

Read Information About the Availability of an In-App Purchase

Get information about the territory availablity for an in-app purchase.

