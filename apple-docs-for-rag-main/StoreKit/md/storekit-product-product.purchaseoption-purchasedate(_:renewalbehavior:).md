

- StoreKit
- Product
- Product.PurchaseOption
-  purchaseDate(\_:renewalBehavior:) 

Type Method

# purchaseDate(\_:renewalBehavior:)

Sets the purchase date for the transaction in the testing environment, and indicates the renewal behavior for an auto-renewable subscription.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func purchaseDate(
    _ date: Date,
    renewalBehavior: Product.PurchaseOption.SubscriptionRenewalBehavior = .renewUntilNow
) -> Product.PurchaseOption
```

## Parameters 

`date`  

The purchase date for the transaction. Specify a date in the past or the current moment. Dates in the future aren’t valid.

`renewalBehavior`  

The renewal behavior for the auto-renewable subscription in this transaction, whether it renews continuously from the purchase date, or it cancels after the first period. By default, the subscription renews.

## Discussion

Use this purchase option when you test your app in Xcode using StoreKit Test and call buyProduct(identifier:options:).

Use this purchase option to create useful transactions for your test cases. For example, use a date in the past with the default `renewalBehavior` to generate a full history of subscription renewals to test. Or, use a date in the past with the Product.PurchaseOption.SubscriptionRenewalBehavior.cancelImmediately behavior to simulate an account of a customer who canceled their subscription.

## See Also

### Setting options for StoreKit Testing in Xcode

enum SubscriptionRenewalBehavior

Renewal options for auto-renewable subscriptions that you purchase in the testing environment.

static func codeOffer(referenceName: String) -> Product.PurchaseOption

Sets an offer code for the transaction in the testing environment.

static func promotionalOffer(id: String) -> Product.PurchaseOption

Sets a promotional offer for the transaction in the testing environment.

