

- StoreKit
- Transaction
-  currency 

Instance Property

# currency

The currency of the price of the product.

iOS 16.0+iPadOS 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@backDeployed(before: iOS 17.2, macOS 14.2, tvOS 17.2, watchOS 10.2, visionOS 1.1)
var currency: Locale.Currency? { get }
```

## Discussion

The currency property represents the currency of the product’s price that the system records at the time of purchase.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

Don’t use currency to infer the storefront. Use the storefront value in the transaction instead.

To access the transaction’s currency on systems earlier than iOS 16, iPadOS 16, macOS 13, tvOS 16, and watchOS 9, use currencyCode.

## See Also

### Getting the product price and currency

var price: Decimal?

The price of the in-app purchase that the system records in the transaction.

