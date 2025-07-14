

- StoreKit
- Transaction
-  appAccountToken 

Instance Property

# appAccountToken

A UUID that associates the transaction with a user on your own service.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let appAccountToken: UUID?
```

## Mentioned in 

Generating a signature for promotional offers

## Discussion

You create an appAccountToken(_:) and send it to the App Store when a customer initiates an in-app purchase. The App Store returns the same value in appAccountToken in the transaction information after the customer completes the purchase.

