

- StoreKit
- Product
- Product.SubscriptionInfo
-  Product.SubscriptionInfo.Status 

Structure

# Product.SubscriptionInfo.Status

The renewal status information for an auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Status
```

## Mentioned in 

Choosing a StoreKit API for In-App Purchases

## Overview

The subscription status provides renewal information signed by the App Store for subscriptions that a customer purchases.

## Topics

### Monitoring subscription status changes

static var updates: Product.SubscriptionInfo.Status.Statuses

The asynchronous sequence that emits status information when a subscription’s status changes.

static var all: AsyncStream&lt;(groupID: String, statuses: [Product.SubscriptionInfo.Status])>

struct Statuses

An asynchronous sequence that listens for new subscription status information.

### Getting subscription status information

let state: Product.SubscriptionInfo.RenewalState

The renewal state of the auto-renewable subscription.

let renewalInfo: VerificationResult&lt;Product.SubscriptionInfo.RenewalInfo>

The signed renewal information for the auto-renewable subscription.

let transaction: VerificationResult&lt;Transaction>

The latest transaction for the subscription group.

struct RenewalInfo

The renewal information for an auto-renewable subscription.

struct RenewalState

The renewal states of auto-renewable subscriptions.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Subscription status and renewal information

struct RenewalInfo

The renewal information for an auto-renewable subscription.

typealias SubscriptionRenewalInfo

Represents the renewal information for an auto-renewable subscription.

struct RenewalState

The renewal states of auto-renewable subscriptions.

typealias SubscriptionRenewalState

The renewal states of auto-renewable subscriptions.

typealias SubscriptionPeriod

Represents the duration of time between subscription renewals.

