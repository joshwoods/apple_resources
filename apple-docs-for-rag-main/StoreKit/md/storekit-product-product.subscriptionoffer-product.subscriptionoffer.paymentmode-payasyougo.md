

- StoreKit
- Product
- Product.SubscriptionOffer
- Product.SubscriptionOffer.PaymentMode
-  payAsYouGo 

Type Property

# payAsYouGo

A payment mode of a product discount that applies over a single billing period or multiple billing periods.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let payAsYouGo: Product.SubscriptionOffer.PaymentMode
```

## Discussion

With a Pay As You Go payment mode, subscribers pay a discounted price for each billing period for the duration of the discount.

## See Also

### Getting the payment modes

static let freeTrial: Product.SubscriptionOffer.PaymentMode

A payment mode of a product discount that indicates a free trial offer.

static let payUpFront: Product.SubscriptionOffer.PaymentMode

A payment mode of a product discount that applies the discount up front.

