

- Advanced Commerce API
-  SubscriptionPriceChangeResponse 

Object

# SubscriptionPriceChangeResponse

A response that contains signed JWS renewal and JWS transaction information after a subscription price change request.

Advanced Commerce API 1.0+

``` source
object SubscriptionPriceChangeResponse
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

This is the response body for the Change Subscription Price endpoint.

## See Also

### Subscription price change from the server

Change Subscription Price

Increase or decrease the price of an auto-renewable subscription, a bundle, or individual items within a subscription at the next renewal.

object SubscriptionPriceChangeRequest

The request body you use to change the price of an auto-renewable subscription.

