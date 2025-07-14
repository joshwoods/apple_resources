

- PassKit (Apple Pay and Wallet)
- PKIssuerProvisioningExtensionPaymentPassEntry
-  init(identifier:title:art:addRequestConfiguration:) 

Initializer

# init(identifier:title:art:addRequestConfiguration:)

Creates a new entry for a payment pass that a user adds to Wallet.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
init?(
    identifier: String,
    title: String,
    art: CGImage,
    addRequestConfiguration configuration: PKAddPaymentPassRequestConfiguration
)
```

## Parameters 

`identifier`  

The value that you use to identify the card.

`title`  

The name for the pass the system displays to the user when they add or select the card.

`art`  

The image that the system displays to the user when they add or select the card.

`configuration`  

The configuration that an PKAddSecureElementPassViewController uses to create a secure pass.

