

- App Store Connect API
-  Read the Billing Grace Period Value 

Web Service Endpoint

# Read the Billing Grace Period Value

Get the Boolean value that represents the billing grace period opt-in state and the duration of the billing grace period.

App Store Connect API 2.0+

## URL

``` source
GET https://api.appstoreconnect.apple.com/v1/subscriptionGracePeriods/{id}
```

## Path Parameters

`id`

`string`

 (Required) 

## Query Parameters

`fields[subscriptionGracePeriods]`

`[string]`

Possible Values: `optIn, sandboxOptIn, duration, renewalType`

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

## Discussion

### Example Request and Response

- Request
- Response

```
https://api.appstoreconnect.apple.com/v1/subscriptionGracePeriods/6446671329
```

```
{
  "data" : {
    "type" : "subscriptionGracePeriods",
    "id" : "6446671329",
    "attributes" : {
      "optIn" : true,
      "sandboxOptIn" : false,
      "duration" : "THREE_DAYS",
      "renewalType" : "ALL_RENEWALS"
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

Modify the Billing Grace Period Opt-in Status and Duration

Change the Boolean value representing the billing grace period opt-in status.

