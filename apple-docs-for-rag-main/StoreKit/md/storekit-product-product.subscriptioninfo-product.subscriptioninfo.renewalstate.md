

- StoreKit
- Product
- Product.SubscriptionInfo
-  Product.SubscriptionInfo.RenewalState 

Structure

# Product.SubscriptionInfo.RenewalState

The renewal states of auto-renewable subscriptions.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct RenewalState
```

## Mentioned in 

Testing In-App Purchases in Xcode

Testing failing subscription renewals and In-App Purchases

## Overview

A subscription’s renewal state indicates whether an auto-renewable subscription is entitled to service. Subscriptions in the subscribed and inGracePeriod states are entitled to service.

Subscriptions in the expired, inBillingRetryPeriod, and revoked states aren’t entitled to service if the customer doesn’t have other Product.SubscriptionInfo.Status items that give them entitlement to service for that subscription. For example, a customer may have a status in the expired state for a subscription that they purchased individually, and another status in the subscribed state for the same subscription, which they get through Family Sharing. In that case, the customer has an entitlement to service for that subscription.

For more information about Family Sharing, see Supporting Family Sharing in your app. For more information about entitlements, see currentEntitlements.

## Topics

### Getting the renewal state

static let subscribed: Product.SubscriptionInfo.RenewalState

The customer is currently subscribed.

static let expired: Product.SubscriptionInfo.RenewalState

The subscription expired.

static let inBillingRetryPeriod: Product.SubscriptionInfo.RenewalState

The subscription is in a billing retry period.

static let inGracePeriod: Product.SubscriptionInfo.RenewalState

The subscription is in a billing grace period state.

static let revoked: Product.SubscriptionInfo.RenewalState

The App Store has revoked the customer’s access to the subscription group.

### Getting a localized description

var localizedDescription: String

A string containing the localized description of the renewal state.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Subscription status and renewal information

struct Status

The renewal status information for an auto-renewable subscription.

struct RenewalInfo

The renewal information for an auto-renewable subscription.

typealias SubscriptionRenewalInfo

Represents the renewal information for an auto-renewable subscription.

typealias SubscriptionRenewalState

The renewal states of auto-renewable subscriptions.

typealias SubscriptionPeriod

Represents the duration of time between subscription renewals.

