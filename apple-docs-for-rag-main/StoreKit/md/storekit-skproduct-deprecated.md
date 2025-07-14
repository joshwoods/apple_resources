

- StoreKit
-  SKProduct Deprecated

Class

# SKProduct

Information about a registered product in App Store Connect.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKProduct
```

Deprecated

Use Product

## Mentioned in 

Implementing promotional offers in your app

Fetching product information from the App Store

Requesting a payment from the App Store

Supporting Family Sharing in your app

## Overview

SKProduct objects are returned as part of an SKProductsResponse object.

## Topics

### Getting the Product Identifier

var productIdentifier: String

The string that identifies the product to the Apple App Store.

### Getting Product Attributes

var localizedDescription: String

A description of the product.

var localizedTitle: String

The name of the product.

var contentVersion: String

A string that identifies the version of the content.

var isFamilyShareable: Bool

A Boolean value that indicates whether the product is available for Family Sharing in App Store Connect.

var contentLengths: [NSNumber]

The total size of the content, in bytes.

### Getting Pricing Information

var price: NSDecimalNumber

The cost of the product in the local currency.

var priceLocale: Locale

The locale used to format the price of the product.

var introductoryPrice: SKProductDiscount?

The object containing introductory price information for the product.

var discounts: [SKProductDiscount]

An array of subscription offers available for the auto-renewable subscription.

class SKProductDiscount

The details of an introductory offer or a promotional offer for an auto-renewable subscription.

### Getting Subscription Information

var subscriptionGroupIdentifier: String?

The identifier of the subscription group to which the subscription belongs.

var subscriptionPeriod: SKProductSubscriptionPeriod?

The period details for products that are subscriptions.

class SKProductSubscriptionPeriod

An object containing the subscription period duration information.

enum PeriodUnit

Values representing the duration of an interval, from a day up to a year.

### Getting Downloadable Content Information

var isDownloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

var downloadContentLengths: [NSNumber]

The lengths of the downloadable files available for this product.

var downloadContentVersion: String

A string that identifies which version of the content is available for download.

var downloadable: Bool

A Boolean value that indicates whether the App Store has downloadable content for this product.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Product information

Loading in-app product identifiers

Load the unique identifiers for your in-app products to retrieve product information from the App Store.

Fetching product information from the App Store

Retrieve up-to-date information about the products for sale in your app to display to your customers.

class SKProductsRequest

An object that can retrieve localized information from the App Store about a specified list of products.

Deprecated

class SKProductsResponse

An App Store response to a request for information about a list of products.

Deprecated

