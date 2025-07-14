

- App Store Connect API
-  Create a Subscription Group Localization 

Web Service Endpoint

# Create a Subscription Group Localization

Create a localized display name and optional custom app name for a subscription group.

App Store Connect API 2.0+

## URL

``` source
POST https://api.appstoreconnect.apple.com/v1/subscriptionGroupLocalizations
```

## HTTP Body

SubscriptionGroupLocalizationCreateRequest

Content-Type: application/json

## Response Codes

` 201 ``Created`

SubscriptionGroupLocalizationResponse

`Created`

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Mentioned in 

Creating auto-renewable subscription groups

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Read Subscription Group Localization Information

Get the specific localized subscription group display name and optional custom app name for a subscription group.

Modify a Subscription Group Localization

Update a specific localized display name and optional custom app name for a subscription group.

Delete a Subscription Group Localization

Delete localized metadata that you configured for a subscription group.

