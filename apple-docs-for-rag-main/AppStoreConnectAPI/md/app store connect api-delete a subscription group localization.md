

- App Store Connect API
-  Delete a Subscription Group Localization 

Web Service Endpoint

# Delete a Subscription Group Localization

Delete localized metadata that you configured for a subscription group.

App Store Connect API 2.0+

## URL

``` source
DELETE https://api.appstoreconnect.apple.com/v1/subscriptionGroupLocalizations/{id}
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

Create a Subscription Group Localization

Create a localized display name and optional custom app name for a subscription group.

Read Subscription Group Localization Information

Get the specific localized subscription group display name and optional custom app name for a subscription group.

Modify a Subscription Group Localization

Update a specific localized display name and optional custom app name for a subscription group.

