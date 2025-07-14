

- External Purchase Server API
-  taxCountry 

Type

# taxCountry

The three-letter country code of the country that collects the taxes for the transaction.

External Purchase Server API 1.0.0+

``` source
string taxCountry
```

## Discussion

Use three-letter ISO 3166-1 Alpha-3 country codes.

## See Also

### Specifying amounts and currency

type amountTaxExclusive

The amount, in milli-units, that the customer paid or was refunded, excluding taxes.

type amountTaxInclusive

The amount, in milli-units, that the customer paid, including taxes.

type netAmountTaxExclusive

The net amount, in milli-units, that you charged the customer, pre-tax, and after deducting all refunds.

type taxAmount

The amount, in milli-units, that the customer paid in taxes.

type pricingCurrency

The currency used in the transaction to bill or refund the customer.

type reportingCurrency

The currency the line item uses to report all amount values.

type exchangeRate

A decimal value that is the exchange rate you use to convert the pricing currency to the reporting currency, when the two currencies differ.

