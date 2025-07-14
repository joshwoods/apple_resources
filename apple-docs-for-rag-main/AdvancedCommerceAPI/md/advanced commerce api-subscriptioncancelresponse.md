

- Advanced Commerce API
-  SubscriptionCancelResponse 

Object

# SubscriptionCancelResponse

The response body for a successful subscription cancellation.

Advanced Commerce API 1.0+

``` source
object SubscriptionCancelResponse
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

This is the response body for the Cancel a Subscription endpoint.

## See Also

### Subscription cancellation from the server

Cancel a Subscription

Turn off automatic renewal to cancel a customer’s auto-renewable subscription.

object SubscriptionCancelRequest

The request body for turning off automatic renewal of a subscription.

