

- External Purchase Server API
-  netAmountTaxExclusive 

Type

# netAmountTaxExclusive

The net amount, in milli-units, that you charged the customer, pre-tax, and after deducting all refunds.

External Purchase Server API 1.0.0+

``` source
int64 netAmountTaxExclusive
```

## Mentioned in 

Reporting corrections

## Discussion

Include this property in the line item to state the net amount in milli-units that you charged the customer, pre-tax, after you account for all refunds and restatements.

Provide all amount field values in milli-units of the currency you state in the reportingCurrency field. One unit of the currency equals 1000 milli-units. For example, if the amount is `€2.99`, the amount in milli-units is `2990`.

To calculate the netAmountTaxExclusive, subtract the refund amount excluding taxes from the original amountTaxExclusive value or from the amount you provided in a restatement, if any.

For example: A customer makes an initial purchase for the pre-tax amount amountTaxExclusive of 1000. They receive a refund of 300. The netAmountTaxExclusive is 700 (which is the original price, 1000, minus the refund of 300).

If you then submit a restatement of the original purchase price to 800, you calculate the netAmountTaxExclusive to be 500, which is the restated price, 800, minus the refund of 300.

This value is used for data validation.

## See Also

### Specifying amounts and currency

type amountTaxExclusive

The amount, in milli-units, that the customer paid or was refunded, excluding taxes.

type amountTaxInclusive

The amount, in milli-units, that the customer paid, including taxes.

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

