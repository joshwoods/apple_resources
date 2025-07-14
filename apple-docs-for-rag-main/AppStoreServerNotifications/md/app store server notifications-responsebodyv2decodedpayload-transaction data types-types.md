

- App Store Server Notifications
- responseBodyV2DecodedPayload
-  Transaction data types 

API Collection

# Transaction data types

Refer to these data types for decoded transaction and renewal information payloads.

## Topics

### Transaction identifiers

type originalTransactionId

The original transaction identifier of a purchase.

type transactionId

The unique identifier for a transaction, such as an In-App Purchase, restored purchase, or subscription renewal.

type webOrderLineItemId

The unique identifier of subscription purchase events across devices, including subscription renewals.

type previousOriginalTransactionId

The original transaction identifer of a subscription before migration.

### App transaction identifier

type appTransactionId

The unique identifier of the app download transaction.

### App information

type bundleId

The bundle identifier of an app.

### Account information

type appAccountToken

A UUID that associates the transaction with a customer on your service.

### Product information

type productId

The product identifier of the In-App Purchase.

type type

The product type of the In-App Purchase.

type subscriptionGroupIdentifier

The identifier of the subscription group that the subscription belongs to.

type quantity

The number of purchased consumable products.

### Product price and currency

type price

The price, in milliunits, of the In-App Purchase that the system records in the transaction.

type currency

The three-letter ISO 4217 currency code for the price of the product.

### Storefront information

type storefront

The three-letter code that represents the country or region associated with the App Store storefront for the purchase.

type storefrontId

An Apple-defined value that uniquely identifies an App Store storefront.

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers to present the better offers first.

type offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

type offerPeriod

The duration of the offer.

type offerType

The type of subscription offer.

type offerDiscountType

The payment mode for a subscription offer for an auto-renewable subscription.

### Purchase dates

type originalPurchaseDate

The purchase date of the transaction associated with the original transaction identifier.

type purchaseDate

The time that the App Store charged the customer’s account for a purchase, a restored product, a subscription, or a subscription renewal after a lapse.

type recentSubscriptionStartDate

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

### Billing status

type isInBillingRetryPeriod

A Boolean value that indicates whether the App Store is attempting to automatically renew a subscription that expired due to a billing issue.

type gracePeriodExpiresDate

The time when the billing grace period for a subscription renewal expires.

### Subscripton renewal and expiration

type autoRenewStatus

The renewal status for an auto-renewable subscription.

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expirationIntent

The reason a subscription expired.

type expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

type isUpgraded

A Boolean value that indicates whether the customer upgraded to another subscription.

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

### Family Sharing

type inAppOwnershipType

A string that describes whether the transaction was purchased by the customer, or is available to them through Family Sharing.

### Price increase status

type priceIncreaseStatus

The status that indicates whether an auto-renewable subscription is subject to a price increase.

### Revocation date and reason

type revocationDate

The UNIX time, in milliseconds, that the App Store refunded the transaction or revoked it from Family Sharing.

type revocationReason

The reason for a refunded transaction.

### Transaction reason

type transactionReason

The cause of a purchase transaction, which indicates whether it’s a customer’s purchase or a renewal for an auto-renewable subscription that the system initiates.

### JWS signature date

type signedDate

The UNIX time, in milliseconds, that the App Store signed the JSON Web Signature data.

### Advanced Commerce API data

Data types for Advanced Commerce API

Objects and data types for transaction that use the Advanced Commerce API.

## See Also

### JWS header and payload data types

object JWSTransactionDecodedPayload

A decoded payload that contains transaction information.

object JWSRenewalInfoDecodedPayload

A decoded payload containing subscription renewal information for an auto-renewable subscription.

object JWSDecodedHeader

A decoded JSON Web Signature header containing transaction or renewal information.

