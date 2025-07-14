

- App Store Server API
-  lastTransactionsItem 

Object

# lastTransactionsItem

The most recent App Store-signed transaction information and App Store-signed renewal information for an auto-renewable subscription.

App Store Server API 1.0+

``` source
object lastTransactionsItem
```

## Properties

`originalTransactionId`

originalTransactionId

The original transaction identifier of the auto-renewable subscription.

`status`

status

The status of the auto-renewable subscription.

`signedRenewalInfo`

JWSRenewalInfo

The subscription renewal information signed by the App Store, in JSON Web Signature (JWS) format.

`signedTransactionInfo`

JWSTransaction

The transaction information signed by the App Store, in JWS format.

## Topics

### Data Types

type originalTransactionId

The original transaction identifier of a purchase.

type status

The status of an auto-renewable subscription.

type JWSRenewalInfo

Subscription renewal information, signed by the App Store, in JSON Web Signature (JWS) format.

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

## See Also

### Object and Data Types

subscriptionGroupIdentifier

