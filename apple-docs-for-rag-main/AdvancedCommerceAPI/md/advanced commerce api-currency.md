

- Advanced Commerce API
-  currency 

Type

# currency

The three-letter ISO 4217 currency code for the price of a product.

Advanced Commerce API 1.0+

``` source
string currency
```

## Mentioned in 

Creating SKUs for your In-App Purchases

Specifying prices for Advanced Commerce SKUs

## Discussion

The currency property contains an ISO 4217 alpha-3 string that represents the currency of the price of a SKU. You provide a currency value each time you create or modify a purchase transaction.

To get the current storefront’s currency in your app:

- In iOS 15 through iOS 17, check the `Product.priceFormatStyle.currencyCode` of the generic product ID that represents your Advanced Commerce product. For more information, see priceFormatStyle.

- In iOS 17 and later, get the currency value using `Storefront.current.currency`.

For a list of regions and currencies that the App Store supports, see Financial reports regions and currencies.

## See Also

### Data types

type description

A string you provide that describes a SKU.

type displayName

A string with a product name that you can localize and is suitable for display to customers.

type effective

A string value that indicates when a requested change to an auto-renewable subscription goes into effect.

type period

The duration of a single cycle of an auto-renewable subscription.

type price

A price, in milliunits of a currency, for an Advanced Commerce API SKU.

type proratedPrice

A prorated price, in milliunits of a currency, for an Advanced Commerce API SKU.

type retainBillingCycle

A Boolean value that determines whether to keep the existing billing cycle with the change you request.

type refundAmount

A refund amount, in milliunits of the currency.

type refundReason

A reason to request a refund.

type refundRiskingPreference

A Boolean value that indicates whether the App Store asks you for consumption data to help inform the refund decision.

type SKU

The product identifier of an in-app purchase product you manage in your own system.

type storefront

A three-letter code that represents the country or region associated with the App Store storefront.

type taxCode

A tax code that applies to a SKU.

type targetProductId

A generic product identifier that represents all Advanced Commerce API products to App Store Connect, which you use when you migrate a product.

type transactionId

A unique identifier that the App Store generates for a transaction.

