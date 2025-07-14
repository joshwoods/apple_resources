

- External Purchase Server API
-  amountTaxExclusive 

Type

# amountTaxExclusive

The amount, in milli-units, that the customer paid or was refunded, excluding taxes.

External Purchase Server API 1.0.0+

``` source
int64 amountTaxExclusive
```

## Discussion

This value must equal amountTaxInclusive minus taxAmount. The `amountTaxExclusive` value is the amount in milli-units that the user paid, excluding taxes. For refunds, it is the amount in milli-units of the refund, excluding taxes.

Provide all amount field values in milli-units of the currency you state in the reportingCurrency field. One unit of the currency equals 1000 milli-units. For example, if the amount is `€2.99`, the amount in milli-units is `2990`.

## See Also

### Specifying amounts and currency

type amountTaxInclusive

The amount, in milli-units, that the customer paid, including taxes.

type netAmountTaxExclusive

The net amount, in milli-units, that you charged the customer, pre-tax, and after deducting all refunds.

type taxAmount

The amount, in milli-units, that the customer paid in taxes.

type taxCountry

The three-letter country code of the country that collects the taxes for the transaction.

type pricingCurrency

The currency used in the transaction to bill or refund the customer.

type reportingCurrency

The currency the line item uses to report all amount values.

type exchangeRate

A decimal value that is the exchange rate you use to convert the pricing currency to the reporting currency, when the two currencies differ.

