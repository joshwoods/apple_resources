

- Advanced Commerce API
-  SubscriptionModifyChangeItem 

Object

# SubscriptionModifyChangeItem

The data your app provides to change an item of an auto-renewable subscription.

Advanced Commerce API 1.0+

``` source
object SubscriptionModifyChangeItem
```

## Properties

`SKU`

SKU

 (Required) 

Maximum length: `128`

`currentSKU`

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

`effective`

effective

 (Required) 

`offer`

Offer

`price`

price

 (Required) 

`proratedPrice`

proratedPrice

`reason`

`string`

 (Required) 

Possible Values: `UPGRADE, DOWNGRADE, APPLY_OFFER`

## See Also

### Subscription modification in the app

object SubscriptionModifyInAppRequest

The request data your app provides to make changes to an auto-renewable subscription.

object SubscriptionModifyAddItem

The data your app provides to add items when it makes changes to an auto-renewable subscription.

object SubscriptionModifyRemoveItem

The data your app provides to remove an item from an auto-renewable subscription.

object SubscriptionModifyPeriodChange

The data your app provides to change the period of an auto-renewable subscription.

