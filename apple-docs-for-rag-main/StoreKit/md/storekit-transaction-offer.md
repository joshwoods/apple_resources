

- StoreKit
- Transaction
-  offer 

Instance Property

# offer

The subscription offer that applies to the transaction, including its offer type, payment mode, and ID.

iOS 17.2+iPadOS 17.2+macOS 14.2+tvOS 17.2+visionOS 1.1+watchOS 10.2+

``` source
let offer: Transaction.Offer?
```

## Mentioned in 

Supporting win-back offers in your app

## Discussion

This value is `nil` if the transaction doesn’t include an offer.

You set up subscription offers for auto-renewable subscriptions in App Store Connect. If a customer redeems an offer, this property contains the offer details, including its type, paymentMode, and id. For more information about the details, see Transaction.Offer.

## See Also

### Identifying subscription offers

struct Offer

The subscription offers that apply to a transaction.

