

- Advanced Commerce API
-  SubscriptionReactivateInAppRequest 

Object

# SubscriptionReactivateInAppRequest

The request your app provides to reactivate a subscription that has automatic renewal turned off.

Advanced Commerce API 1.0+

``` source
object SubscriptionReactivateInAppRequest
```

## Properties

`items`

SubscriptionReactivateItem

`operation`

`string`

 (Required) 

Value: `REACTIVATE_SUBSCRIPTION`

`requestInfo`

RequestInfo

 (Required) 

`storefront`

storefront

`transactionId`

transactionId

 (Required) 

`version`

version

 (Required) 

## See Also

### Subscription reactivation in the app

object SubscriptionReactivateItem

An item in a subscription to reactive.

