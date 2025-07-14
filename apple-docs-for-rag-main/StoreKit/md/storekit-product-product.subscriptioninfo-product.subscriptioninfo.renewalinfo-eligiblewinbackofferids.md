

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  eligibleWinBackOfferIDs 

Instance Property

# eligibleWinBackOfferIDs

An array of strings that represent identifiers of win-back offers that the customer is eligible to redeem, sorted with the best offers first.

iOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
let eligibleWinBackOfferIDs: [String]
```

## Mentioned in 

Merchandising win-back offers in your app

## Discussion

Use this list to select an eligible win-back offer for a customer. The array contains strings that represent offer identifiers for win-back offers. You provide the offer identifier in App Store Connect when you configure a win-back offer.

The App Store sets the order of the eligible win-back offer IDs for each customer, with the best offer first. The order takes into account the available offers you configure in App Store Connect for the customer’s most recent subscription in the subscription group. Subscriptions in a Billing Grace Period or billing retry state aren’t eligible for win-back offers.

Get the complete offer details by searching for the identifier in the winBackOffers property of the Product.SubscriptionInfo instance. To add the offer to a purchase when a customer accepts the offer, use the winBackOffer(_:) purchase option. For more information, see Supporting win-back offers in your app.

When you test win-back offers with StoreKit Testing in Xcode, the system lists the offers in no particular order. For more information, see Testing win-back offers in Xcode.

You can also use the App Store Server API to get a list of eligible win-back offers, on your server. For more information, see Get All Subscription Statuses and eligibleWinBackOfferIds.

For information about configuring win-back offers in App Store Connect, see Set up win-back offers.

## See Also

### Getting subscription offers

let offer: Transaction.Offer?

A subscription offer that applies to the transaction at the next renewal period.

struct Offer

The subscription offers that apply to a transaction.

