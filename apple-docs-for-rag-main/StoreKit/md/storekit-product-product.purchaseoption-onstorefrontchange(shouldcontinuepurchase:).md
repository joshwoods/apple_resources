

- StoreKit
- Product
- Product.PurchaseOption
-  onStorefrontChange(shouldContinuePurchase:) 

Type Method

# onStorefrontChange(shouldContinuePurchase:)

Indicates whether a transaction needs to continue if the App Store storefront changes on the device during the transaction.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
static func onStorefrontChange(shouldContinuePurchase: @escaping (Storefront) -> Bool) -> Product.PurchaseOption
```

## Parameters 

`shouldContinuePurchase`  

A closure that returns a Boolean value to indicate whether the purchase needs to continue when the App Store storefront changes to the storefront value during a transaction.

## Return Value

Product.PurchaseOption

## Discussion

The default value is `true` if this option isn’t added to the purchase.

