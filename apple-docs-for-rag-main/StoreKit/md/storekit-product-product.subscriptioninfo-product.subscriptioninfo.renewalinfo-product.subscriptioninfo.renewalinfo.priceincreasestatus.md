

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus 

Enumeration

# Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus

Status values that indicate whether an auto-renewable subscription is subject to a price increase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@frozen
enum PriceIncreaseStatus
```

## Overview

For more information, see Managing Price Increases for Auto-Renewable Subscriptions.

## Topics

### Getting Price Increase Status

case noIncreasePending

There’s no pending price increase for the auto-renewable subscription.

case agreed

The auto-renewable subscription is subject to a price increase.

case pending

The customer hasn’t yet responded to an auto-renewable subscription price increase that requires customer consent.

### Getting a Localized Description

var localizedDescription: String

A string containing the localized description of the price increase status.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the price increase status

Managing Price Increases for Auto-Renewable Subscriptions

Identify the price increase status for auto-renewable subscriptions in your app and on your server.

let priceIncreaseStatus: Product.SubscriptionInfo.RenewalInfo.PriceIncreaseStatus

The status that indicates whether the auto-renewable subscription is subject to a price increase.

