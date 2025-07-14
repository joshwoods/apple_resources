

- CryptoTokenKit
- TKSmartCardToken
-  init(smartCard:aid:instanceID:tokenDriver:) 

Initializer

# init(smartCard:aid:instanceID:tokenDriver:)

Initializes a smart card token with the specified smart card, application identifier, and token driver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    smartCard: TKSmartCard,
    aid AID: Data?,
    instanceID: String,
    tokenDriver: TKSmartCardTokenDriver
)
```

## Parameters 

`smartCard`  

The smart card on which the created token should operate.

`AID`  

The ISO 7816-4 application identifier for the smart card.

`instanceID`  

A unique, persistent identifier for this token. This value is typically generated from the serial number of the target hardware.

`tokenDriver`  

The driver associated with the created token.

## Discussion

This is the designated initializer.

