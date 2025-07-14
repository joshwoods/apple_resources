

- StoreKit
- AdvancedCommerceProduct
- AdvancedCommerceProduct.PurchaseOption
-  onStorefrontChange(shouldContinuePurchase:) 

Type Method

# onStorefrontChange(shouldContinuePurchase:)

A closure that determines whether the transaction continues if the device’s App Store storefront changes during a transaction.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
static func onStorefrontChange(shouldContinuePurchase: @escaping (Storefront) -> Bool) -> AdvancedCommerceProduct.PurchaseOption
```

## Parameters 

`shouldContinuePurchase`  

A closure that returns a Boolean value that determines whether the purchase continues when the storefront changes to `Storefront` during the purchase process.

## Discussion

The default is `true` if you don’t include this option in the purchase options.

