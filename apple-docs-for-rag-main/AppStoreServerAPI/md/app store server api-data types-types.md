

- App Store Server API
-  Data types 

API Collection

# Data types

Refer to these data types for decoded transaction and renewal information payloads.

## Topics

### Environment

type environment

The server environment, either sandbox or production.

### Transaction identifiers

type originalTransactionId

The original transaction identifier of a purchase.

type transactionId

The unique identifier for a transaction, such as an In-App Purchase, restored In-App Purchase, or subscription renewal.

type webOrderLineItemId

The unique identifier of subscription-purchase events across devices, including renewals.

### App transaction identifier

type appTransactionId

The unique identifier of the app download transaction.

### App information

type appAppleId

The unique identifier of an app in the App Store.

type bundleId

The bundle identifier of an app.

### Account information

type appAccountToken

The UUID that an app optionally generates to map a customer’s In-App Purchase with its resulting App Store transaction.

### Product information

type productId

The unique identifier of the product, which you create in App Store Connect.

type type

The type of In-App Purchase products you can offer in your app.

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

The three-letter code that represents the country or region associated with the App Store storefront of the purchase.

type storefrontId

An Apple-defined value that uniquely identifies an App Store storefront.

### Subscription offers

type eligibleWinBackOfferIds

An array of win-back offer identifiers that a customer is eligible to redeem, which sorts the identifiers with the best offers first.

type offerIdentifier

The string identifier of a subscription offer that you create in App Store Connect.

type offerPeriod

The duration of the offer.

type offerType

The type of subscription offer.

type offerDiscountType

The payment mode for subscription offers on an auto-renewable subscription.

### Purchase dates

type originalPurchaseDate

The purchase date of the transaction associated with the original transaction identifier.

type purchaseDate

The time that the App Store charged the customer’s account for an In-App Purchase, a restored In-App Purchase, a subscription, or a subscription renewal after a lapse.

type recentSubscriptionStartDate

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

### Billing status

type isInBillingRetryPeriod

A Boolean value that indicates whether the App Store is attempting to automatically renew an expired subscription.

type gracePeriodExpiresDate

The time when the Billing Grace Period for subscription renewals expires.

### Subscription renewal and expiration

type autoRenewStatus

The renewal status for an auto-renewable subscription.

type autoRenewProductId

The identifier of the product that renews at the next billing period.

type expirationIntent

The reason an auto-renewable subscription expired.

type expiresDate

The UNIX time, in milliseconds, an auto-renewable subscription purchase expires or renews.

type isUpgraded

The Boolean value that indicates whether the customer upgraded to another subscription.

type renewalDate

The UNIX time, in milliseconds, when the most recent auto-renewable subscription purchase expires.

type renewalPrice

The renewal price, in milliunits, of the auto-renewable subscription that renews at the next billing period.

type status

The status of an auto-renewable subscription.

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

### JWS headers and payloads

type JWSTransaction

Transaction information signed by the App Store, in JSON Web Signature (JWS) Compact Serialization format.

type JWSRenewalInfo

Subscription renewal information, signed by the App Store, in JSON Web Signature (JWS) format.

object JWSDecodedHeader

A decoded JSON Web Signature (JWS) header containing transaction or renewal information.

object JWSTransactionDecodedPayload

A decoded payload that contains transaction information.

object JWSRenewalInfoDecodedPayload

A decoded payload containing subscription renewal information for an auto-renewable subscription.

