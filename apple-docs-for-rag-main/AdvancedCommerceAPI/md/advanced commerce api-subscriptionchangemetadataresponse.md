

- Advanced Commerce API
-  SubscriptionChangeMetadataResponse 

Object

# SubscriptionChangeMetadataResponse

The response body for a successful subscription metadata change.

Advanced Commerce API 1.1+

``` source
object SubscriptionChangeMetadataResponse
```

## Properties

`signedRenewalInfo`

JWSRenewalInfo

 (Required) 

Subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format.

`signedTransactionInfo`

JWSTransaction

 (Required) 

Transaction information signed by the App Store, in JWS Compact Serialization format.

## Discussion

This is the response body for the Change Subscription Metadata endpoint.

## See Also

### Subscription metadata changes from the server

Change Subscription Metadata

Update the SKU, display name, and description associated with a subscription, without affecting the subscription’s billing or its service.

object SubscriptionChangeMetadataRequest

The request body you provide to change the metadata of a subscription.

object SubscriptionChangeMetadataDescriptors

The subscription metadata to change, specifically the description and display name.

object SubscriptionChangeMetadataItem

The metadata to change for an item, specifically its SKU, description, and display name.

