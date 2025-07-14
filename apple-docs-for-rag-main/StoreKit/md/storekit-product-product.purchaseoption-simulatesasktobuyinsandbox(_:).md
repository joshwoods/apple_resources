

- StoreKit
- Product
- Product.PurchaseOption
-  simulatesAskToBuyInSandbox(\_:) 

Type Method

# simulatesAskToBuyInSandbox(\_:)

Simulates an Ask to Buy scenario when testing your app in the sandbox environment.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func simulatesAskToBuyInSandbox(_ simulateAskToBuy: Bool) -> Product.PurchaseOption
```

## Parameters 

`simulateAskToBuy`  

Set to `true` to simulate a child’s account asking permission to make a purchase.

## Return Value

An instance of Product.PurchaseOption to use in purchase(options:).

## Discussion

For information about testing Ask to Buy scenarios, see Testing at all stages of development with Xcode and the sandbox.

For information about purchases made using Ask to Buy, see Approve what kids buy with Ask to Buy.

