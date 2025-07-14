

- StoreKit
- Transaction
-  isUpgraded 

Instance Property

# isUpgraded

A Boolean that indicates whether the user upgraded to another subscription.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
let isUpgraded: Bool
```

## Discussion

If isUpgraded is `true`, the user has upgraded the subscription represented by this transaction to another subscription. This value appears in the transaction only when the value is `true`. To determine the service that the customer is entitled to, look for another transaction that has a subscription with a higher level of service.

## See Also

### Getting purchase details

let ownershipType: Transaction.OwnershipType

A value that indicates whether the transaction was purchased by the user, or is made available to them through Family Sharing.

struct OwnershipType

The types the system uses to describe whether the user purchased the product or it’s available to them through Family Sharing.

let purchasedQuantity: Int

The number of consumable products purchased.

