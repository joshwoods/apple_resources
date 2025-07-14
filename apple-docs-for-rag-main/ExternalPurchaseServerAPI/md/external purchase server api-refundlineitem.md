

- External Purchase Server API
-  RefundLineItem 

Object

# RefundLineItem

The line item that indicates a refund transaction.

External Purchase Server API 1.0.0+

``` source
object RefundLineItem
```

## Properties

`lineItemId`

lineItemId

 (Required) 

A unique identifier for the transaction, that you determine. The value must be unique per app. Using UUIDs is recommended. Reuse a `lineItemId` only to submit a correction for a previously submitted line item.

`referenceLineItemId`

referenceLineItemId

 (Required) 

The lineItemId of the initial purchase transaction that receives a refund.

`creationDate`

creationDate

 (Required) 

The UNIX date, in milliseconds, you completed the transaction.

`restatement`

restatement

Set to `true` to indicate that this line item is correcting (restating) a refund line item that you previously submitted. For more information, see Reporting corrections.

Default: `false`

`erroneouslySubmitted`

erroneouslySubmitted

Set to `true` to indicate that you previously submitted the line item in error. Set the `restatement` field to `true` also. For more information, see Reporting corrections.

Default: `false`

`pricingCurrency`

pricingCurrency

 (Required) 

The currency the transaction used to charge or refund the customer. For more information, see pricingCurrency.

`reportingCurrency`

reportingCurrency

 (Required) 

The currency you use to report all the amount fields, including `amountTaxExclusive`, `amountTaxInclusive`, `netAmountTaxExclusive`, and `taxAmount`. For more information, see reportingCurrency.

`exchangeRate`

exchangeRate

The exchange rate you use to calculate the amounts, from the pricing currency to the reporting currency, if the customer is billed in an unsupported currency. For more information, see exchangeRate.

`amountTaxExclusive`

amountTaxExclusive

 (Required) 

The amount that the customer paid, excluding taxes, that you state in milli-units of the reporting currency. For more information, see amountTaxExclusive.

`amountTaxInclusive`

amountTaxInclusive

 (Required) 

The amount that the customer paid, including taxes, that you state in milli-units of the reporting currency. For more information, see amountTaxInclusive.

`netAmountTaxExclusive`

netAmountTaxExclusive

 (Required) 

The net amount the customer was charged, accurate to the current line item, that you state in milli-units of the reporting currency. This amount excludes tax, and accounts for all refunds and restatements. For more information, see netAmountTaxExclusive.

`taxAmount`

taxAmount

 (Required) 

The amount the customer paid in taxes, that you state in milli-units of the reporting currency. For more information, see taxAmount.

`taxCountry`

taxCountry

 (Required) 

The country code of the country for which taxes were paid on the purchase. For more information, see taxCountry.

`eventType`

eventType

 (Required) 

Use `REFUND`.

## Mentioned in 

Reporting tokens with transactions

Reporting corrections

## Discussion

Use a `RefundLineItem` to report either:

- A refund for a purchase transaction you previously submitted, or

- A correction to a refund you previously submitted

For more information about sending a report that includes refund line items, see Reporting tokens with transactions.

Report chargebacks as a refund.

## See Also

### External purchase report transactions

Reporting tokens with transactions

Create reports for external purchase tokens that result in completed transactions, including one-time charges, subscriptions and renewals, and refunds.

Reporting corrections

Submit a report with corrections if you find errors in, or have adjustments to, a successfully submitted transaction.

object OneTimeBuyLineItem

The line item that indicates a one-time charge transaction.

object SubscriptionBuyLineItem

The line item that indicates a subscription-related event or transaction.

Line item fields

Properties that describe a single transaction or correction in an external purchase report.

