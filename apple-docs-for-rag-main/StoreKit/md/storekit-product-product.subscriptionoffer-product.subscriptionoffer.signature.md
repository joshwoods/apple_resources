

- StoreKit
- Product
- Product.SubscriptionOffer
-  Product.SubscriptionOffer.Signature 

Structure

# Product.SubscriptionOffer.Signature

A cryptographic signature for a promotional offer.

iOS 17.4+iPadOS 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Signature
```

## Overview

For information about promotional offers, see Implementing promotional offers in your app.

The App Store Server Library provides a function that produces signatures for promotional offers. For more information, see Simplifying your implementation by using the App Store Server Library.

## Topics

### Creating subscription offer signatures

init(keyID: String, nonce: UUID, timestamp: Int, signature: Data)

Creates a subscription offer signature instance.

### Getting signature elements

var keyID: String

A string that identifies the private key you use to generate the cryptographic signature.

var nonce: UUID

A one-time UUID your server generates for the promotional offer.

var signature: Data

A cryptographic signature your server generates to sign a promotional offer for an auto-renewable subscription.

var timestamp: Int

A timestamp your server generates in UNIX time format, in milliseconds, that indicates the time the server generated the signature.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

