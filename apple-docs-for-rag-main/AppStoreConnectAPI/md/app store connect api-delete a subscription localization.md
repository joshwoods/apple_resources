

- App Store Connect API
-  Delete a Subscription Localization 

Web Service Endpoint

# Delete a Subscription Localization

Delete localized metadata that you configured for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/subscriptionLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Response Codes

` 204 ``No Content`

`No Content`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Read Subscription Localization Information

Get the specific localized metadata for an auto-renewable subscription.

Create a Subscription Localization

Create a localized display name and description for an auto-renewable subscription.

Modify a Subscription Localization

Update a specific localized subscription display name and description for an auto-renewable subscription.

