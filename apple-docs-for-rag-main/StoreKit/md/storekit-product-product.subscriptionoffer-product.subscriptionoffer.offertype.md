

- StoreKit
- Product
- Product.SubscriptionOffer
-  Product.SubscriptionOffer.OfferType 

Structure

# Product.SubscriptionOffer.OfferType

The types of offers for auto-renewable subscriptions.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct OfferType
```

## Topics

### Getting offer types

static let introductory: Product.SubscriptionOffer.OfferType

An introductory offer for an auto-renewable subscription.

static let promotional: Product.SubscriptionOffer.OfferType

A promotional offer for an auto-renewable subscription.

static let winBack: Product.SubscriptionOffer.OfferType

A win-back offer for an auto-renewable subscription.

### Getting a localized description

var localizedDescription: String

A string that contains the localized description of the offer type.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Subscription offers and offer codes

Supporting win-back offers in your app

Re-engage previous subscribers with a free or discounted offer for an auto-renewable subscription, for a specific duration.

Merchandising win-back offers in your app

Present win-back offers to eligible customers in your app with the win-back offer sheet or by implementing custom merchandising.

Supporting subscription offer codes in your app

Provide subscription service for customers who redeem offer codes through the App Store or within your app.

struct SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

