

- StoreKit
- Product
- Product.SubscriptionInfo
- Product.SubscriptionInfo.RenewalInfo
-  currency 

Instance Property

# currency

The currency of the subscription’s renewal price.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@backDeployed(before: iOS 18.0, macOS 15.0, tvOS 18.0, watchOS 11.0, visionOS 2.0)
var currency: Locale.Currency? { get }
```

## Discussion

The currency value applies to the product’s renewalPrice instance.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

Don’t use currency to infer the storefront. Use the storefront value in the transaction instead.

To access the renewal price currency on systems earlier than iOS 16, iPadOS 16, macOS 13, tvOS 16, and watchOS 9, use currencyCode.

## See Also

### Getting the renewal price and currency

var renewalPrice: Decimal?

The renewal price of the auto-renewable subscription that renews at the next billing period.

