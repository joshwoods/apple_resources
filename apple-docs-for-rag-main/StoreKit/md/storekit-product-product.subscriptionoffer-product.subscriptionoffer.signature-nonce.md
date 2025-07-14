

- StoreKit
- Product
- Product.SubscriptionOffer
- Product.SubscriptionOffer.Signature
-  nonce 

Instance Property

# nonce

A one-time UUID your server generates for the promotional offer.

iOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
var nonce: UUID
```

## See Also

### Getting signature elements

var keyID: String

A string that identifies the private key you use to generate the cryptographic signature.

var signature: Data

A cryptographic signature your server generates to sign a promotional offer for an auto-renewable subscription.

var timestamp: Int

A timestamp your server generates in UNIX time format, in milliseconds, that indicates the time the server generated the signature.

