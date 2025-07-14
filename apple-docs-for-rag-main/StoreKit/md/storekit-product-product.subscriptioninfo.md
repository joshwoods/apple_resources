

- StoreKit
- Product
-  Product.SubscriptionInfo 

Structure

# Product.SubscriptionInfo

Information about an auto-renewable subscription, such as its status, period, subscription group, and subscription offer details.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SubscriptionInfo
```

## Mentioned in 

Merchandising win-back offers in your app

Choosing a StoreKit API for In-App Purchases

## Topics

### Determining the subscription status

var status: [Product.SubscriptionInfo.Status]

An array that contains status information for a subscription group, including renewal and transaction information.

static func status(for: String) async throws -> [Product.SubscriptionInfo.Status]

Gets the subscription status for a subscription group identifier.

struct Status

The renewal status information for an auto-renewable subscription.

### Identifying the subscription group

let subscriptionGroupID: String

The subscription group identifier for this subscription.

var groupDisplayName: String

The localized name of the subscription group, suitable for display.

var groupLevel: Int

The rank of the subscription relative to other subscriptions in the same subscription group.

### Getting the subscription period

let subscriptionPeriod: Product.SubscriptionPeriod

The duration of time between subscription renewals.

struct SubscriptionPeriod

Values that represent the duration of time between subscription renewals.

### Getting introductory offer details

var isEligibleForIntroOffer: Bool

A Boolean value that indicates whether the customer is eligible for an introductory offer.

static func isEligibleForIntroOffer(for: String) async -> Bool

Returns a Boolean value that determines the customer’s eligibility for an introductory offer within the provided subscription group.

let introductoryOffer: Product.SubscriptionOffer?

Information about the introductory offer available for the auto-renewable subscription.

struct SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

### Getting win-back offer details

let winBackOffers: [Product.SubscriptionOffer]

An array of available win-back offers for the auto-renewable subscription that you configured in App Store Connect.

### Getting promotional offer details

let promotionalOffers: [Product.SubscriptionOffer]

An array of promotional offers available for the auto-renewable subscription.

### Structures

struct RenewalInfo

The renewal information for an auto-renewable subscription.

struct RenewalState

The renewal states of auto-renewable subscriptions.

### Type Methods

static func status(transactionID: UInt64) async throws -> SubscriptionStatus?

Gets the subscription status for a transaction ID.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Product and subscription information

Implementing a store in your app using the StoreKit API

Offer In-App Purchases and manage entitlements using signed transactions and status information.

struct Product

Information about a product that you configure in App Store Connect.

typealias SubscriptionInfo

Information about an auto-renewable subscription.

typealias SubscriptionStatus

Represents the renewal status information for an auto-renewable subscription.

