

- Advanced Commerce API
-  SubscriptionModifyAddItem 

Object

# SubscriptionModifyAddItem

The data your app provides to add items when it makes changes to an auto-renewable subscription.

Advanced Commerce API 1.0+

``` source
object SubscriptionModifyAddItem
```

## Properties

`SKU`

SKU

 (Required) 

Maximum length: `128`

`description`

description

 (Required) 

Maximum length: `45`

`displayName`

displayName

 (Required) 

Maximum length: `30`

`offer`

Offer

`price`

price

 (Required) 

`proratedPrice`

proratedPrice

## See Also

### Subscription modification in the app

object SubscriptionModifyInAppRequest

The request data your app provides to make changes to an auto-renewable subscription.

object SubscriptionModifyChangeItem

The data your app provides to change an item of an auto-renewable subscription.

object SubscriptionModifyRemoveItem

The data your app provides to remove an item from an auto-renewable subscription.

object SubscriptionModifyPeriodChange

The data your app provides to change the period of an auto-renewable subscription.

