

- App Store Connect API
-  Read Subscription Group Localization Information 

Web Service Endpoint

# Read Subscription Group Localization Information

Get the specific localized subscription group display name and optional custom app name for a subscription group.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionGroupLocalizations/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionGroupLocalizations]`

`[string]`

Possible Values: `name, customAppName, locale, state, subscriptionGroup`

`include`

`[string]`

Value: `subscriptionGroup`

## Response Codes

` 200 ``OK`

SubscriptionGroupLocalizationResponse

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

Create a Subscription Group Localization

Create a localized display name and optional custom app name for a subscription group.

Modify a Subscription Group Localization

Update a specific localized display name and optional custom app name for a subscription group.

Delete a Subscription Group Localization

Delete localized metadata that you configured for a subscription group.

