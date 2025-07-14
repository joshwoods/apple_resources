

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  Product.SubscriptionInfo.RenewalInfo.AdvancedCommerceInfo 

Structure

# Product.SubscriptionInfo.RenewalInfo.AdvancedCommerceInfo

Renewal information for subscriptions that use the Advanced Commerce API.

iOS 18.4+iPadOS 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
struct AdvancedCommerceInfo
```

## Topics

### Structures

struct Item

The developer-defined product that was purchased.

### Instance Properties

let consistencyToken: String

let description: String

let displayName: String

let items: [Product.SubscriptionInfo.RenewalInfo.AdvancedCommerceInfo.Item]

The items included in this subscription.

let period: SubscriptionPeriod

let requestReferenceID: String

let taxCode: String

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Getting renewal information for Advanced Commerce API

let advancedCommerceInfo: Product.SubscriptionInfo.RenewalInfo.AdvancedCommerceInfo?

Renewal information for a subscription that uses the Advanced Commerce API.

