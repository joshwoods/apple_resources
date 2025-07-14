

- StoreKit
- Product
- Product.PurchaseOption
-  Product.PurchaseOption.SubscriptionRenewalBehavior 

Enumeration

# Product.PurchaseOption.SubscriptionRenewalBehavior

Renewal options for auto-renewable subscriptions that you purchase in the testing environment.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum SubscriptionRenewalBehavior
```

## Overview

Use the subscription renewal behavior values when you use the purchaseDate option to test your app in Xcode using StoreKit Test.

## Topics

### Renewal behaviors in the testing environment

case cancelImmediately

A subscription-renewal behavior in the testing environment that cancels the subscription, resulting in only one subscription period.

case renewUntilNow

A subscription-renewal behavior in the testing environment that allows the subscription to renew continuously, up to the current date.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Setting options for StoreKit Testing in Xcode

static func purchaseDate(Date, renewalBehavior: Product.PurchaseOption.SubscriptionRenewalBehavior) -> Product.PurchaseOption

Sets the purchase date for the transaction in the testing environment, and indicates the renewal behavior for an auto-renewable subscription.

static func codeOffer(referenceName: String) -> Product.PurchaseOption

Sets an offer code for the transaction in the testing environment.

static func promotionalOffer(id: String) -> Product.PurchaseOption

Sets a promotional offer for the transaction in the testing environment.

