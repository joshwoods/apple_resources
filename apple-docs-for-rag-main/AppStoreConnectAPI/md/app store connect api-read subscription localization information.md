

- App Store Connect API
-  Read Subscription Localization Information 

Web Service Endpoint

# Read Subscription Localization Information

Get the specific localized metadata for an auto-renewable subscription.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionLocalizations]`

`[string]`

Possible Values: `name, locale, description, state, subscription`

`include`

`[string]`

Value: `subscription`

## Response Codes

` 200 ``OK`

SubscriptionLocalizationResponse

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

Create a Subscription Localization

Create a localized display name and description for an auto-renewable subscription.

Modify a Subscription Localization

Update a specific localized subscription display name and description for an auto-renewable subscription.

Delete a Subscription Localization

Delete localized metadata that you configured for an auto-renewable subscription.

