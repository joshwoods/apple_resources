

- StoreKit
- Transaction
- Transaction.OfferType
-  winBack 

Type Property

# winBack

A win-back offer for an auto-renewable subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 18.0, macOS 15.0, tvOS 18.0, watchOS 11.0, visionOS 2.0)
static var winBack: Transaction.OfferType { get }
```

## Discussion

For more information about win-back offers, see Set up win-back offers.

The raw value of the winBack offer type is `4`.

## See Also

### Getting offer types

static let introductory: Transaction.OfferType

An introductory offer for an auto-renewable subscription.

static let promotional: Transaction.OfferType

A promotional offer for an auto-renewable subscription.

static let code: Transaction.OfferType

An offer with a subscription offer code for an auto-renewable subscription.

