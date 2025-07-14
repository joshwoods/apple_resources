

- StoreKit
- Product
- Product.PurchaseOption
-  promotionalOffer(id:) 

Type Method

# promotionalOffer(id:)

Sets a promotional offer for the transaction in the testing environment.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func promotionalOffer(id identifier: String) -> Product.PurchaseOption
```

## Parameters 

`identifier`  

The identifier of the promotional offer to apply to the transaction. You need to set up identifiers in your StoreKit configuration file.

## Discussion

Use this purchase option when you test your app in Xcode using StoreKit Test and call buyProduct(identifier:options:). This method makes it possible to test promotional offers without supplying a signature.

Set up the promotional offer identifiers that you use in this call in your StoreKit configuration file. For more information, see Setting up StoreKit Testing in Xcode.

When you apply this option, the purchase transaction simulates a customer redeeming a promotional offer, and includes the promotional offer you specify.

## See Also

### Setting options for StoreKit Testing in Xcode

static func purchaseDate(Date, renewalBehavior: Product.PurchaseOption.SubscriptionRenewalBehavior) -> Product.PurchaseOption

Sets the purchase date for the transaction in the testing environment, and indicates the renewal behavior for an auto-renewable subscription.

enum SubscriptionRenewalBehavior

Renewal options for auto-renewable subscriptions that you purchase in the testing environment.

static func codeOffer(referenceName: String) -> Product.PurchaseOption

Sets an offer code for the transaction in the testing environment.

