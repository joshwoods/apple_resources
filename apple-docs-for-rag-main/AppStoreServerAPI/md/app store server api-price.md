

- App Store Server API
-  price 

Type

# price

The price, in milliunits, of the In-App Purchase that the system records in the transaction.

App Store Server API 1.10+

``` source
int64 price
```

## Mentioned in 

App Store Server API changelog

## Discussion

This value represents the price, in milliunits of the currency, of the In-App Purchase that the system records in the transaction. One unit of the currency equals 1000 milliunits.

The `price` value reflects all of the following:

- The price you configured in App Store Connect, which the system records on the purchase date (purchaseDate).

- The discount from a subscription offer in the offerIdentifier, if the transaction includes an offer.

- The quantity of a consumable in-app purchase. The price value shows the total amount of the transaction for the quantity the customer purchased.

The following table shows some examples of the `price` and currency parameters based on sample prices you might configure in App Store Connect:

| Configured price in App Store Connect | `price` parameter | `currency` parameter |
|----|----|----|
| \$1.99 (U.S. dollar) | 1990 | USD |
| KRW 3300 (South Korean won) | 3300000 | KRW |
| JPY 300 (Japanese yen) | 300000 | JPY |

To determine the storefront, use the storefront value in the transaction. Don’t use the `currency` value to infer the storefront.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

For more information on how you set prices, see Set a price and Set a price for an in-app purchase.

## See Also

### Product price and currency

type currency

The three-letter ISO 4217 currency code for the price of the product.

