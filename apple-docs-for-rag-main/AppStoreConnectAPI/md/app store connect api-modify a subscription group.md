

- App Store Connect API
-  Modify a Subscription Group 

Web Service Endpoint

# Modify a Subscription Group

Update the reference name for a specific subscription group.

App Store Connect API 2.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/subscriptionGroups/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

SubscriptionGroupUpdateRequest

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionGroupResponse

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

` 409 ``Conflict`

ErrorResponse

`Conflict`

Content-Type: application/json

` 422 `

ErrorResponse

Content-Type: application/json

## Discussion

Note

Changes that you make to product metadata with the App Store Connect API can take up to 1 hour to appear in the sandbox environment.

## See Also

### Endpoints

Create a Subscription Group

Create a subscription group for an app.

List All Subscription Groups for an App

Get a list of subscription groups for a specific app.

Read Subscription Group Information

Get the details of a specific subscription group.

Delete a Subscription Group

Delete a specific empty subscription group.

List All Subscription Group Localizations

Get a list of all localized metadata for a specific subscription group.

List All Subscriptions for a Subscription Group

Get a list of all auto-renewable subscriptions in a subscription group.

