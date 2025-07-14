

- StoreKit
- Transaction
-  price 

Instance Property

# price

The price of the in-app purchase that the system records in the transaction.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@backDeployed(before: iOS 17.2, macOS 14.2, tvOS 17.2, watchOS 10.2, visionOS 1.1)
var price: Decimal? { get }
```

## Discussion

This value represents the price of the in-app purchase, in units of the currency, that the system records in the transaction. The price value reflects all of the following:

- The price you configured in App Store Connect, which the system records on the purchase date (purchaseDate).

- The discount from a subscription offer in the offer property, if the transaction includes an offer.

- The purchasedQuantity of a consumable in-app purchase. The price value shows the total amount of the transaction for the quantity that the customer purchased.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

The decoded payloads of jwsRepresentation and the JWSTransaction strings from the App Store server APIs contain price fields specified in *milliunits* of the currency. StoreKit represents the price value in *units* of the currency. Take care not to confuse these two representations when working with both APIs.

You configure prices in App Store Connect. For more information, see Set a price for an in-app purchase.

## See Also

### Getting the product price and currency

var currency: Locale.Currency?

The currency of the price of the product.

