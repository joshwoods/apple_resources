

- Advanced Commerce API
-  SubscriptionChangeMetadataRequest 

Object

# SubscriptionChangeMetadataRequest

The request body you provide to change the metadata of a subscription.

Advanced Commerce API 1.1+

``` source
object SubscriptionChangeMetadataRequest
```

## Properties

`descriptors`

SubscriptionChangeMetadataDescriptors

`items`

`[`SubscriptionChangeMetadataItem`]`

`requestInfo`

RequestInfo

 (Required) 

`storefront`

storefront

`taxCode`

taxCode

## See Also

### Subscription metadata changes from the server

Change Subscription Metadata

Update the SKU, display name, and description associated with a subscription, without affecting the subscription’s billing or its service.

object SubscriptionChangeMetadataResponse

The response body for a successful subscription metadata change.

object SubscriptionChangeMetadataDescriptors

The subscription metadata to change, specifically the description and display name.

object SubscriptionChangeMetadataItem

The metadata to change for an item, specifically its SKU, description, and display name.

