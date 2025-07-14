

- StoreKit
- Product
-  Product.PurchaseResult 

Enumeration

# Product.PurchaseResult

The result of a purchase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum PurchaseResult
```

## Overview

The value of the purchase result represents the state of the purchase. When successful, the associated value contains a VerificationResult of the transaction. The following example illustrates calling purchase(options:) on a Product value, checking the purchase status, and inspecting information about a successful transaction.

```
let result = try await product.purchase()
switch result {
case .success(let verificationResult):
    switch verificationResult {
    case .verified(let transaction):
        // Give the user access to purchased content.
        ...
        // Complete the transaction after providing
        // the user access to the content.
        await transaction.finish()
    case .unverified(let transaction, let verificationError):
        // Handle unverified transactions based 
        // on your business model.
        ...
    }
case .pending:
    // The purchase requires action from the customer. 
    // If the transaction completes, 
    // it's available through Transaction.updates.
    break
case .userCancelled:
    // The user canceled the purchase.
    break
@unknown default:
    break
}

```

## Topics

### Getting the Purchase Results

case success(VerificationResult&lt;Transaction>)

The purchase succeeded and results in a transaction.

case userCancelled

The user canceled the purchase.

case pending

The purchase is pending, and requires action from the customer.

## Relationships

### Conforms To

- Sendable

## See Also

### Purchase requests and results

struct PurchaseAction

An action that starts an In-App Purchase.

func purchase(options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

