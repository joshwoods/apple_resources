

- StoreKit
- Product
-  Product.PurchaseOption 

Structure

# Product.PurchaseOption

Optional settings for a product purchase that add account information, purchase details, and offers, or that specify behaviors.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct PurchaseOption
```

## Mentioned in 

Generating JWS to sign App Store requests

## Overview

Associate purchase options with an in-app purchase when you call the methods to initiate a purchase, such as purchase(options:) or purchase(confirmIn:options:). Use the testing-specific options with StoreKit Test or in the sandbox testing environment.

Purchase options enable you to provide additional information for the purchase, such as an app account token, promotional offer, win back offer, and quantity. You can also use purchase options to indicate how the transaction behaves if the storefront changes, and to indicate whether the transaction is eligible for an introductory offer.

Important

Purchases fail if a purchase option is invalid, and can result in the purchase method throwing a StoreKitError or Product.PurchaseError.

### Use purchase options during testing

In the sandbox testing environment, use simulatesAskToBuyInSandbox(_:) to test Ask To Buy scenarios.

In the Xcode testing environment with StoreKit Test, use the following testing-specific purchase options when you call buyProduct(identifier:options:):

- Use codeOffer(referenceName:) and promotionalOffer(id:) to simulate customers redeeming the offers.

- Use purchaseDate(_:renewalBehavior:) to control the transaction date and subscription renewal behavior.

## Topics

### Setting the purchase options

static func appAccountToken(UUID) -> Product.PurchaseOption

Sets a UUID to associate the purchase with an account in your system.

static func winBackOffer(Product.SubscriptionOffer) -> Product.PurchaseOption

Sets a win-back offer to apply to the purchase.

static func promotionalOffer(offerID: String, keyID: String, nonce: UUID, signature: Data, timestamp: Int) -> Product.PurchaseOption

Applies a promotional offer for an auto-renewable subscription.

static func promotionalOffer(offerID: String, signature: Product.SubscriptionOffer.Signature) -> Product.PurchaseOption

static func quantity(Int) -> Product.PurchaseOption

Indicates the quantity of items the customer is purchasing.

### Specifying the behavior for storefront changes

static func onStorefrontChange(shouldContinuePurchase: (Storefront) -> Bool) -> Product.PurchaseOption

Indicates whether a transaction needs to continue if the App Store storefront changes on the device during the transaction.

### Specifying eligibility for an introductory offer

static func introductoryOfferEligibility(compactJWS: String) -> Product.PurchaseOption

Set the eligibility of an introductory offer for a purchase.

### Setting options for StoreKit Testing in Xcode

static func purchaseDate(Date, renewalBehavior: Product.PurchaseOption.SubscriptionRenewalBehavior) -> Product.PurchaseOption

Sets the purchase date for the transaction in the testing environment, and indicates the renewal behavior for an auto-renewable subscription.

enum SubscriptionRenewalBehavior

Renewal options for auto-renewable subscriptions that you purchase in the testing environment.

static func codeOffer(referenceName: String) -> Product.PurchaseOption

Sets an offer code for the transaction in the testing environment.

static func promotionalOffer(id: String) -> Product.PurchaseOption

Sets a promotional offer for the transaction in the testing environment.

### Setting options for sandbox testing

static func simulatesAskToBuyInSandbox(Bool) -> Product.PurchaseOption

Simulates an Ask to Buy scenario when testing your app in the sandbox environment.

### Setting custom purchase options

static func custom(key: String, value: Data) -> Product.PurchaseOption

Adds data for a custom key to a purchase.

static func custom(key: String, value: String) -> Product.PurchaseOption

Adds a string for a custom key to a purchase.

static func custom(key: String, value: Bool) -> Product.PurchaseOption

Adds a Boolean value for a custom key to a purchase.

static func custom(key: String, value: Double) -> Product.PurchaseOption

Adds a number for a custom key to a purchase.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
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

enum PurchaseResult

The result of a purchase.

enum PurchaseError

Error information for product purchase errors.

