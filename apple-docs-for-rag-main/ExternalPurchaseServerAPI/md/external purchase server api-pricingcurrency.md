

- External Purchase Server API
-  pricingCurrency 

Type

# pricingCurrency

The currency used in the transaction to bill or refund the customer.

External Purchase Server API 1.0.0+

``` source
string pricingCurrency
```

## Discussion

Maximum length: 128. Use a three-letter ISO 4217 currency code to specify the currency.

The `pricingCurrency` is the currency used in the transaction to charge or refund the customer. The pricing currency affects your reporting currency, reportingCurrency, which you use to report all amount values.

The currencies Apple supports are listed as allowed values on the reportingCurrency page.

Important

If your `pricingCurrency` isn’t a currency that Apple supports, you must use EUR or USD as the reportingCurrency.

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

type taxCountry

The three-letter country code of the country that collects the taxes for the transaction.

type reportingCurrency

The currency the line item uses to report all amount values.

type exchangeRate

A decimal value that is the exchange rate you use to convert the pricing currency to the reporting currency, when the two currencies differ.

