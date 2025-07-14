

- StoreKit
- Product
- Product.SubscriptionInfo
-  Product.SubscriptionInfo.RenewalInfo 

Structure

# Product.SubscriptionInfo.RenewalInfo

The renewal information for an auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct RenewalInfo
```

## Mentioned in 

Supporting subscription offer codes in your app

Testing failing subscription renewals and In-App Purchases

Merchandising win-back offers in your app

## Overview

`Product.SubscriptionInfo.RenewalInfo` provides information about the next subscription renewal period. Check the state to determine whether the subscription will be active (subscribed), expired, or in another state at the next renewal period.

## Topics

### Getting the environment

let environment: AppStore.Environment

The server environment that signs the renewal information for an auto-renewable subscription.

### Getting the transaction ID

let originalTransactionID: UInt64

The transaction identifier of the original purchase.

### Identifying the account

var appAccountToken: UUID?

The app account token you provided during the subscription purchase, if one exists.

var appTransactionID: String

The unique identifier of the app download transaction.

### Getting the product ID

let currentProductID: String

The subscription product ID that the customer is subscribed to.

### Getting subscription dates

var recentSubscriptionStartDate: Date

The earliest start date of a subscription in a series of auto-renewable subscription purchases that ignores all lapses of paid service shorter than 60 days.

var renewalDate: Date?

The UNIX time, in milliseconds, that the most recent auto-renewable subscription purchase expires.

### Getting the renewal or expiration state

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let autoRenewPreference: String?

The product ID of the auto-renewable subscription that will automatically renew.

let willAutoRenew: Bool

A Boolean value that indicates whether the subscription automatically renews in the next period.

let expirationReason: Product.SubscriptionInfo.RenewalInfo.ExpirationReason?

The reason the auto-renewable subscription expired.

struct ExpirationReason

The reasons for auto-renewable subscription expirations.

### Getting subscription offers

let offer: Transaction.Offer?

A subscription offer that applies to the transaction at the next renewal period.

struct Offer

The subscription offers that apply to a transaction.

let eligibleWinBackOfferIDs: [String]

An array of strings that represent identifiers of win-back offers that the customer is eligible to redeem, sorted with the best offers first.

### Getting the renewal price and currency

var renewalPrice: Decimal?

The renewal price of the auto-renewable subscription that renews at the next billing period.

var currency: Locale.Currency?

The currency of the subscription’s renewal price.

### Getting billing status

let isInBillingRetry: Bool

A Boolean value that indicates whether an auto-renewable subscription is in the billing retry period.

let gracePeriodExpirationDate: Date?

The date the billing grace period expires for the auto-renewable subscription.

### Getting the price increase status

Managing Price Increases for Auto-Renewable Subscriptions

Identify the price increase status for auto-renewable subscriptions in your app and on your server.

let priceIncreaseStatus: Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus

The status that indicates whether the auto-renewable subscription is subject to a price increase.

enum PriceIncreaseStatus

Status values that indicate whether an auto-renewable subscription is subject to a price increase.

### Verifying subscription renewal information

let deviceVerification: Data

The device verification value to use to verify whether the renewal information belongs to the device.

let deviceVerificationNonce: UUID

The UUID to use to compute the device verification value.

let signedDate: Date

The date that the App Store signed the JWS renewal information.

### Getting subscription renewal info in JSON format

var jsonRepresentation: Data

The JSON representation of the subscription renewal information.

### Getting renewal information for Advanced Commerce API

let advancedCommerceInfo: Product.SubscriptionInfo.RenewalInfo.AdvancedCommerceInfo?

Renewal information for a subscription that uses the Advanced Commerce API.

struct AdvancedCommerceInfo

Renewal information for subscriptions that use the Advanced Commerce API.

### Deprecated

var environmentStringRepresentation: String

The string representation of the server environment that signs the renewal information for an auto-renewable subscription.

Deprecated

var offerID: String?

A string that identifies an offer applied to the next subscription period.

Deprecated

var offerType: Transaction.OfferType?

The subscription offer type for the next subscription period.

Deprecated

var currencyCode: String?

The three-letter ISO 4217 currency code for the price of the product.

Deprecated

var offerPaymentModeStringRepresentation: String?Deprecated

var offerPeriodStringRepresentation: String?

The string representation of the subscription offer period applied to the next billing period.

Deprecated

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Subscription status and renewal information

struct Status

The renewal status information for an auto-renewable subscription.

typealias SubscriptionRenewalInfo

Represents the renewal information for an auto-renewable subscription.

struct RenewalState

The renewal states of auto-renewable subscriptions.

typealias SubscriptionRenewalState

The renewal states of auto-renewable subscriptions.

typealias SubscriptionPeriod

Represents the duration of time between subscription renewals.

