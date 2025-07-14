

- StoreKit
- In-App Purchase
- Transaction
-  Transaction properties 

API Collection

# Transaction properties

The properties of a transaction, including identifiers, purchase and revocation dates and details, status, and offer details.

## Topics

### Getting the environment and storefront

let environment: AppStore.Environment

The server environment that generates and signs the transaction.

let storefront: Storefront

The App Store storefront associated with the transaction.

### Getting the original transaction identifier

let originalID: UInt64

The original transaction identifier of a purchase.

let originalPurchaseDate: Date

The date of purchase for the original transaction.

### Identifying a transaction

let id: UInt64

The unique identifier for the transaction.

let webOrderLineItemID: String?

A unique ID that identifies subscription purchase events across devices, including subscription renewals.

### Identifying the app and product

let appBundleID: String

The bundle identifier for the app.

let productID: String

The product identifier of the in-app purchase.

let productType: Product.ProductType

The type of the in-app purchase.

let subscriptionGroupID: String?

The identifier of the subscription group that the subscription belongs to.

### Getting purchase and expiration dates

let purchaseDate: Date

The date that the App Store charged the user’s account for a purchased or restored product, or for a subscription purchase or renewal after a lapse.

let expirationDate: Date?

The date the subscription expires or renews.

### Getting the product price and currency

var price: Decimal?

The price of the in-app purchase that the system records in the transaction.

var currency: Locale.Currency?

The currency of the price of the product.

### Getting purchase details

let isUpgraded: Bool

A Boolean that indicates whether the user upgraded to another subscription.

let ownershipType: Transaction.OwnershipType

A value that indicates whether the transaction was purchased by the user, or is made available to them through Family Sharing.

struct OwnershipType

The types the system uses to describe whether the user purchased the product or it’s available to them through Family Sharing.

let purchasedQuantity: Int

The number of consumable products purchased.

### Getting subscription status

var subscriptionStatus: Product.SubscriptionInfo.Status?

An array that contains status information for a subscription group, including renewal and transaction information.

### Getting transaction reason

let reason: Transaction.Reason

The cause of the purchase transaction, whether it’s a customer’s purchase or an auto-renewable subscription renewal that the system initiates.

struct Reason

A cause of a purchase transaction, indicating whether it’s a customer’s purchase or an auto-renewable subscription renewal that the system initiates.

### Identifying subscription offers

let offer: Transaction.Offer?

The subscription offer that applies to the transaction, including its offer type, payment mode, and ID.

struct Offer

The subscription offers that apply to a transaction.

### Getting revocation status

let revocationDate: Date?

The date that the App Store refunded the transaction or revoked it from Family Sharing.

let revocationReason: Transaction.RevocationReason?

The reason that the App Store refunded the transaction or revoked it from Family Sharing.

struct RevocationReason

Reasons that describe why the App Store may refund a transaction or revoke it from Family Sharing.

### Correlating transactions with accounts

let appAccountToken: UUID?

A UUID that associates the transaction with a user on your own service.

### Getting the transaction information in JSON format

var jsonRepresentation: Data

The JSON representation of the transaction information.

### Deprecated

var currencyCode: String?

The three-letter ISO 4217 currency code for the price of the product.

Deprecated

var environmentStringRepresentation: String

A string representation of the server environment.

Deprecated

var offerID: String?

A string that identifies an offer applied to the current subscription.

Deprecated

var offerPaymentModeStringRepresentation: String?

The string representation of the payment mode for a subscription offer.

Deprecated

var offerType: Transaction.OfferType?

The subscription offer type for the current subscription period.

Deprecated

var reasonStringRepresentation: String

The string representation of the transaction reason.

Deprecated

var storefrontCountryCode: String

The three-letter code that represents the country or region associated with the App Store storefront of the purchase.

Deprecated

## See Also

### Transaction properties

var appTransactionID: String

The unique identifier of the app download transaction.

