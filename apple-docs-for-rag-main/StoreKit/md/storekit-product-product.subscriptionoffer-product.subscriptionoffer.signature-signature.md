

- StoreKit
- Product
- Product.SubscriptionOffer
- Product.SubscriptionOffer.Signature
-  signature 

Instance Property

# signature

A cryptographic signature your server generates to sign a promotional offer for an auto-renewable subscription.

iOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
var signature: Data
```

## See Also

### Getting signature elements

var keyID: String

A string that identifies the private key you use to generate the cryptographic signature.

var nonce: UUID

A one-time UUID your server generates for the promotional offer.

var timestamp: Int

A timestamp your server generates in UNIX time format, in milliseconds, that indicates the time the server generated the signature.

