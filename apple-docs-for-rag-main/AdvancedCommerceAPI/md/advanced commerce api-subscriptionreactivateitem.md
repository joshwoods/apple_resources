

- Advanced Commerce API
-  SubscriptionReactivateItem 

Object

# SubscriptionReactivateItem

An item in a subscription to reactive.

Advanced Commerce API 1.1+

``` source
object SubscriptionReactivateItem
```

## Properties

`SKU`

SKU

 (Required) 

The SKU of the item to reactivate.

Maximum length: `128`

## Discussion

This object is part of the SubscriptionReactivateInAppRequest that your app uses to reactivate a subscription that would otherwise expire.

## See Also

### Subscription reactivation in the app

object SubscriptionReactivateInAppRequest

The request your app provides to reactivate a subscription that has automatic renewal turned off.

