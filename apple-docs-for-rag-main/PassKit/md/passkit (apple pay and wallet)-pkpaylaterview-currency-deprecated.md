

- PassKit (Apple Pay and Wallet)
- PKPayLaterView
-  currency Deprecated

Instance Property

# currency

The ISO-4217 currency code for the country or region of the merchant’s principle place of business.

iOS 17.0+iPadOS 17.0+visionOS

``` source
@MainActor @preconcurrency
var currency: Locale.Currency { get set }
```

Deprecated

Apple Pay Later is deprecated.

## Discussion

Use the ISO-4217 currency code that represents the location of the merchant’s principal place of business.

## See Also

### Accessing information about the transaction

var amount: Decimal

The decimal value that represents the amount of the customer’s shopping cart or item pricing.

Deprecated

