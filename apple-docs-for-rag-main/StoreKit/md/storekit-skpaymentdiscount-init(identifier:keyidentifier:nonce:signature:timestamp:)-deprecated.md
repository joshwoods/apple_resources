

- StoreKit
- SKPaymentDiscount
-  init(identifier:keyIdentifier:nonce:signature:timestamp:) Deprecated

Initializer

# init(identifier:keyIdentifier:nonce:signature:timestamp:)

Initializes the payment discount with a signature and the parameters used by the signature.

iOS 12.2–18.0DeprecatediPadOS 12.2–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14.4–15.0DeprecatedtvOS 12.2–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
init(
    identifier: String,
    keyIdentifier: String,
    nonce: UUID,
    signature: String,
    timestamp: NSNumber
)
```

Deprecated

Create a Product.PurchaseOption.promotionalOffer to use in Product.purchase(confirmIn:options:)

