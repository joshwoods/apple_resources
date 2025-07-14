

- StoreKit Test
- SKTestTransaction
-  expirationDate 

Instance Property

# expirationDate

The date a subscription expires.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var expirationDate: Date? { get }
```

## Discussion

The test environment sets the expiration date based on the subscription settings in your active StoreKit configuration file.

## See Also

### Getting Dates

var purchaseDate: Date

The date of purchase for the transaction.

var cancelDate: Date?

The date when the system refunded the transaction.

