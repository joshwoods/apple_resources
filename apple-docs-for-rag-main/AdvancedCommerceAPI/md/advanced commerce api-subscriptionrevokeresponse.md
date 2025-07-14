

- Advanced Commerce API
-  SubscriptionRevokeResponse 

Object

# SubscriptionRevokeResponse

The response body for a successful revoke-subscription request.

Advanced Commerce API 1.1+

``` source
object SubscriptionRevokeResponse
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

This is the response body for the Revoke Subscription endpoint.

## See Also

### Subscription revocation from the server

Revoke Subscription

Immediately cancel a customer’s subscription and all the items that are included in the subscription, and request a full or prorated refund.

object SubscriptionRevokeRequest

The request body you provide to terminate a subscription and all its items immediately.

