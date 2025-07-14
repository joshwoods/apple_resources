

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  offer 

Instance Property

# offer

A subscription offer that applies to the transaction at the next renewal period.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let offer: Transaction.Offer?
```

## Discussion

This value is populated if a customer redeems a subscription offer that applies to more than one subscription period.

This value is `nil` if there’s no subscription offer.

## See Also

### Getting subscription offers

struct Offer

The subscription offers that apply to a transaction.

let eligibleWinBackOfferIDs: [String]

An array of strings that represent identifiers of win-back offers that the customer is eligible to redeem, sorted with the best offers first.

