

- App Store Connect API
-  Modify the Billing Grace Period Opt-in Status and Duration 

Web Service Endpoint

# Modify the Billing Grace Period Opt-in Status and Duration

Change the Boolean value representing the billing grace period opt-in status.

App Store Connect API 2.0+

## URL

``` source
PATCH https://api.appstoreconnect.apple.com/v1/subscriptionGracePeriods/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## HTTP Body

SubscriptionGracePeriodUpdateRequest

There are now new duration options that can be set by using SubscriptionGracePeriodDuration

Content-Type: application/json

## Response Codes

` 200 ``OK`

SubscriptionGracePeriodResponse

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

## Mentioned in 

Managing auto-renewable subscriptions

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/subscriptionGracePeriods/6446671329     
-d $'{
  "data": {
    "type": "subscriptionGracePeriods",
    "id": "6446671329",
    "attributes": {
      "sandboxOptIn": true,
      "optIn": true,
      "renewalType": "PAID_TO_PAID_ONLY",
      "duration": "TWENTY_EIGHT_DAYS"
    }
  }
}'
```

```
{
  "data" : {
    "type" : "subscriptionGracePeriods",
    "id" : "6446671329",
    "attributes" : {
      "optIn" : true,
      "sandboxOptIn" : true,
      "duration" : "TWENTY_EIGHT_DAYS",
      "renewalType" : "PAID_TO_PAID_ONLY"
    },
    "links" : {
      "self" : "https://api.appstoreconnect.apple.com/v1/subscriptionGracePeriods/6446671329"
    }
  },
  "links" : {
    "self" : "https://api.appstoreconnect.apple.com/v1/subscriptionGracePeriods/6446671329"
  }
}
```

## See Also

### Endpoints

Read the Billing Grace Period Value for an App

Get the Boolean value that represents the grace period opt-in state for your app.

Read the Billing Grace Period Value

Get the Boolean value that represents the billing grace period opt-in state and the duration of the billing grace period.

