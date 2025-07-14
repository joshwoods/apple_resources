

- Advanced Commerce API
-  SubscriptionCreateItem 

Object

# SubscriptionCreateItem

The data that describes a subscription item.

Advanced Commerce API 1.0+

``` source
object SubscriptionCreateItem
```

## Properties

`SKU`

SKU

 (Required) 

The item’s product identifier, which you define.

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

## See Also

### Subscription creation in the app

object SubscriptionCreateRequest

The metadata your app provides when a customer purchases an auto-renewable subscription.

