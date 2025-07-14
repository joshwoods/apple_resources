

- StoreKit
- Transaction
-  all(for:) 

Type Method

# all(for:)

Gets all the transactions associated with this product ID.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
static func all(for productID: String) -> Transaction.Transactions
```

## Parameters 

`productID`  

Identifies the product to filter the transaction cache against.

## Return Value

A sequence containing all transactions for the given product.

