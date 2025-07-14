

- Advanced Commerce API
-  SubscriptionRevokeRequest 

Object

# SubscriptionRevokeRequest

The request body you provide to terminate a subscription and all its items immediately.

Advanced Commerce API 1.1+

``` source
object SubscriptionRevokeRequest
```

## Properties

`refundReason`

refundReason

 (Required) 

`refundRiskingPreference`

refundRiskingPreference

 (Required) 

`refundType`

`string`

 (Required) 

Possible Values: `FULL, PRORATED`

`requestInfo`

RequestInfo

 (Required) 

`storefront`

storefront

## Discussion

This is the request body for the Revoke Subscription endpoint.

## See Also

### Subscription revocation from the server

Revoke Subscription

Immediately cancel a customer’s subscription and all the items that are included in the subscription, and request a full or prorated refund.

object SubscriptionRevokeResponse

The response body for a successful revoke-subscription request.

