

- StoreKit
- Transaction
-  originalID 

Instance Property

# originalID

The original transaction identifier of a purchase.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let originalID: UInt64
```

## Discussion

The original transaction identifier, originalID, is identical to id except when the user restores a purchase or renews a transaction. You can use this value to:

- Identify one or more renewals for the same subscription.

- Differentiate a purchase transaction from a restore or a renewal transaction. For restore and renewal transactions, the original transaction identifier, originalID, and transaction identifier, id, differ.

- Match a transaction in the app with a transaction you receive on your server in an App Store Server Notifications event.

## See Also

### Getting the original transaction identifier

let originalPurchaseDate: Date

The date of purchase for the original transaction.

