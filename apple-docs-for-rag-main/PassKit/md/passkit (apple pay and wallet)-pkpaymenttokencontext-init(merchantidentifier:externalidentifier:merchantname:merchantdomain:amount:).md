

- PassKit (Apple Pay and Wallet)
- PKPaymentTokenContext
-  init(merchantIdentifier:externalIdentifier:merchantName:merchantDomain:amount:) 

Initializer

# init(merchantIdentifier:externalIdentifier:merchantName:merchantDomain:amount:)

Create a payment token context for a single merchant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    merchantIdentifier: String,
    externalIdentifier: String,
    merchantName: String,
    merchantDomain: String?,
    amount: NSDecimalNumber
)
```

## Parameters 

`merchantIdentifier`  

The Apple Pay merchant identifier.

`externalIdentifier`  

An external identifier for the merchant.

`merchantName`  

The merchant’s display name that the Apple Pay server associates with the payment token.

`merchantDomain`  

The merchant’s top-level domain that the Apple Pay server associates with the payment token.

`amount`  

The amount to authorize for the payment token.

