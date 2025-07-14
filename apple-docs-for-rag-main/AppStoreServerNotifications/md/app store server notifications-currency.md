

- App Store Server Notifications
-  currency 

Type

# currency

The three-letter ISO 4217 currency code for the price of the product.

App Store Server Notifications 2.9+

``` source
string currency
```

## Mentioned in 

App Store Server Notifications changelog

## Discussion

The currency property contains an ISO 4217 alpha-3 string that represents the currency of the price of the product.

Important

For financial and accounting purposes, use the App Store Connect reporting tools. For more information, see Download financial reports and Overview of reporting tools.

Don’t use the currency value to infer the storefront. Use the storefront value in the transaction instead.

For more information on how you set prices, see Set a price and Set a price for an in-app purchase.

## See Also

### Product price and currency

type price

The price, in milliunits, of the In-App Purchase that the system records in the transaction.

