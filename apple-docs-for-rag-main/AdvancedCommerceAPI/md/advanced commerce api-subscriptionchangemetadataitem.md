

- Advanced Commerce API
-  SubscriptionChangeMetadataItem 

Object

# SubscriptionChangeMetadataItem

The metadata to change for an item, specifically its SKU, description, and display name.

Advanced Commerce API 1.1+

``` source
object SubscriptionChangeMetadataItem
```

## Properties

`SKU`

SKU

The new SKU of the item.

Maximum length: `128`

`currentSKU`

SKU

 (Required) 

The original SKU of the item.

Maximum length: `128`

`description`

description

The new description for the item.

Maximum length: `45`

`displayName`

displayName

The new display name for the item.

Maximum length: `30`

`effective`

effective

 (Required) 

The string that determines when the metadata change goes into effect.

## See Also

### Subscription metadata changes from the server

Change Subscription Metadata

Update the SKU, display name, and description associated with a subscription, without affecting the subscription’s billing or its service.

object SubscriptionChangeMetadataRequest

The request body you provide to change the metadata of a subscription.

object SubscriptionChangeMetadataResponse

The response body for a successful subscription metadata change.

object SubscriptionChangeMetadataDescriptors

The subscription metadata to change, specifically the description and display name.

