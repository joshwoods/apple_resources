

- StoreKit
- Product
- Product.PurchaseOption
-  codeOffer(referenceName:) 

Type Method

# codeOffer(referenceName:)

Sets an offer code for the transaction in the testing environment.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func codeOffer(referenceName: String) -> Product.PurchaseOption
```

## Parameters 

`referenceName`  

The reference name of the offer code to apply to the transaction. You need to set up offer codes in your StoreKit configuration file.

## Discussion

Use this purchase option when you test your app in Xcode using StoreKit Test and call buyProduct(identifier:options:).

Set up the offer codes to use in this call in your StoreKit configuration file. For more information, see Setting up StoreKit Testing in Xcode.

When you apply this option, the purchase transaction simulates a customer redeeming an offer code and includes the offer code you specify.

## See Also

### Setting options for StoreKit Testing in Xcode

static func purchaseDate(Date, renewalBehavior: Product.PurchaseOption.SubscriptionRenewalBehavior) -> Product.PurchaseOption

Sets the purchase date for the transaction in the testing environment, and indicates the renewal behavior for an auto-renewable subscription.

enum SubscriptionRenewalBehavior

Renewal options for auto-renewable subscriptions that you purchase in the testing environment.

static func promotionalOffer(id: String) -> Product.PurchaseOption

Sets a promotional offer for the transaction in the testing environment.

