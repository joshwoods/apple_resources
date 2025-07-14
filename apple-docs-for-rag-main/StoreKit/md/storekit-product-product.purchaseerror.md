

- StoreKit
- Product
-  Product.PurchaseError 

Enumeration

# Product.PurchaseError

Error information for product purchase errors.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum PurchaseError
```

## Overview

The purchase(options:) function may throw a purchase error.

## Topics

### Getting Purchase Error Codes

case invalidOfferIdentifier

The promotional offer identifier provided in the purchase options is invalid.

case productUnavailable

The product isn’t available.

case purchaseNotAllowed

The user isn’t allowed to make purchases.

case ineligibleForOffer

The user isn’t eligible for the offer.

case invalidOfferPrice

The price of the offer isn’t valid.

case invalidOfferSignature

The offer signature isn’t valid.

case invalidQuantity

The quantity to purchase is invalid.

case missingOfferParameters

The offer parameters are missing.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

## See Also

### Purchasing a product

func purchase(options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

func purchase(confirmIn: some UIScene, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Initiates a purchase for the product with the App Store and displays the confirmation sheet.

func purchase(confirmIn: UIViewController, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Processes a purchase for the product.

func purchase(confirmIn: NSWindow, options: Set&lt;Product.PurchaseOption>) async throws -> Product.PurchaseResult

Processes a purchase for the product.

struct PurchaseOption

Optional settings for a product purchase that add account information, purchase details, and offers, or that specify behaviors.

enum PurchaseResult

The result of a purchase.

