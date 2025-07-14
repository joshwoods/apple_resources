

- StoreKit
- Product
-  Product.SubscriptionPeriod 

Structure

# Product.SubscriptionPeriod

Values that represent the duration of time between subscription renewals.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct SubscriptionPeriod
```

## Overview

Use the value and the unit together to determine the subscription period. For example, if the unit is Product.SubscriptionPeriod.Unit.month, and the value is `3`, the subscription period is three months.

## Topics

### Getting the subscription period

let value: Int

The number of period units.

let unit: Product.SubscriptionPeriod.Unit

The increment of time for the subscription period.

enum Unit

Units of time that describe subscription periods.

### Getting the period date range

func dateRange(referenceDate: Date) -> Range&lt;Date>

The calculated date range of a subscription period, starting at the reference date.

### Getting subscription periods

static var everySixMonths: Product.SubscriptionPeriod

static var everyThreeDays: Product.SubscriptionPeriod

static var everyThreeMonths: Product.SubscriptionPeriod

static var everyTwoMonths: Product.SubscriptionPeriod

static var everyTwoWeeks: Product.SubscriptionPeriod

static var monthly: Product.SubscriptionPeriod

static var weekly: Product.SubscriptionPeriod

static var yearly: Product.SubscriptionPeriod

### Formatting the subscription period

func formatted&lt;S>(S, referenceDate: Date) -> S.FormatOutput

Formats the subscription period using a format style that takes a date range as an input.

func formatted&lt;S>(S, referenceDate: Date) -> S.FormatOutput

Formats the subscription period using a format style that takes a duration as an input.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting subscription information

let subscription: Product.SubscriptionInfo?

The subscription information for an auto-renewable subscripton.

struct SubscriptionInfo

Information about an auto-renewable subscription, such as its status, period, subscription group, and subscription offer details.

struct SubscriptionOffer

Information about a subscription offer that you configure in App Store Connect.

struct Status

The renewal status information for an auto-renewable subscription.

