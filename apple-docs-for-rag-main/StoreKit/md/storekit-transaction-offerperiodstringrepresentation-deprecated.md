

- StoreKit
- Transaction
-  offerPeriodStringRepresentation Deprecated

Instance Property

# offerPeriodStringRepresentation

The string representation of the offer period applied to the subscription offer for this transaction.

iOS 15.0–18.4DeprecatediPadOS 15.0–18.4DeprecatedmacOS 12.0–15.4DeprecatedtvOS 15.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 8.0–11.4Deprecated

``` source
@backDeployed(before: iOS 18.4, macOS 15.4, tvOS 18.4, watchOS 11.4, visionOS 2.4)
var offerPeriodStringRepresentation: String? { get }
```

Deprecated

Use the offer property instead.

## Discussion

This value is present only for subscriptions that include an offer.

Important

In rare cases, the property might return a sentinel `nil` value. One possible reason is using StoreKit Testing in Xcode; try testing on a device with a newer OS. Another reason might be a critical server error.

