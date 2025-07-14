

- StoreKit
-  AdvancedCommerceProduct 

Structure

# AdvancedCommerceProduct

A product configured as a generic SKU in App Store Connect for use with the Advanced Commerce API.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct AdvancedCommerceProduct
```

## Topics

### Getting the product ID and type

typealias ProductType

let type: AdvancedCommerceProduct.ProductType

The type of the product.

### Initiating purchases

struct PurchaseOption

func purchase(compactJWS: String, confirmIn: NSWindow, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, confirmIn: UIViewController, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

func purchase(compactJWS: String, options: Set&lt;AdvancedCommerceProduct.PurchaseOption>) async throws -> AdvancedCommerceProduct.PurchaseResult

Processes a purchase for the product.

typealias PurchaseResult

### Getting transactions and entitlements

var allTransactions: Transaction.Transactions

All transactions associated with the generic product ID.

var currentEntitlements: Transaction.Transactions

The transactions that entitle the customer to Advanced Commerce Items purchased using the generic product ID.

var latestTransaction: VerificationResult&lt;Transaction>?

The most recent transaction associated with the generic product ID, if it exists.

### Initializing an instance

init(id: AdvancedCommerceProduct.ID) async throws

Creates an Advanced Commerce product.

### Handling errors

struct InvalidRequestError

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Advanced Commerce API interactions

Sending Advanced Commerce API requests from your app

Send Advanced Commerce API requests from your app that you authorize with a JSON Web Signature (JWS) you generate on your server.

Generating JWS to sign App Store requests

Create signed JSON Web Signature (JWS) strings on your server to authorize your API requests in your app.

