

- StoreKit Test
- SKTestTransaction
-  cancelDate 

Instance Property

# cancelDate

The date when the system refunded the transaction.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var cancelDate: Date? { get }
```

## Discussion

The cancelDate is equivalent to the revocationDate in Transaction. The system sets the cancelDate if it refunds or revokes the in-app purchase. Otherwise, the value is `nil`.

A subscription can have a `nil` cancelDate and be inactive if its expiration date passed.

The system doesn’t set cancelDate if the user turns off auto-renewing for the subscription. If the user upgrades the subscription, the system sets isUpgraded in Transaction to `true` and sends a new transaction for the upgraded subscription. The system doesn’t set cancelDate in this case.

## See Also

### Getting Dates

var purchaseDate: Date

The date of purchase for the transaction.

var expirationDate: Date?

The date a subscription expires.

