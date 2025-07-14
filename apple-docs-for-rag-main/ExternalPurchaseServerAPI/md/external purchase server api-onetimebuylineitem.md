

- External Purchase Server API
-  OneTimeBuyLineItem 

Object

# OneTimeBuyLineItem

The line item that indicates a one-time charge transaction.

External Purchase Server API 1.0.0+

``` source
object OneTimeBuyLineItem
```

## Properties

`lineItemId`

lineItemId

 (Required) 

A unique identifier for the transaction, that you determine. The value must be unique per app. Using UUIDs is recommended. Reuse a `lineItemId` only to submit a restatement for a previously submitted line item.

`creationDate`

creationDate

 (Required) 

The UNIX date, in milliseconds, that the customer authorized the purchase.

`restatement`

restatement

Set to `true` to indicate that this line item is correcting (restating) a line item that you previously submitted. For more information, see Reporting corrections.

Default: `false`

`erroneouslySubmitted`

erroneouslySubmitted

Set to `true` to indicate that you previously submitted the line item erroneously. Set the `restatement` field to `true` also. For more information, see Reporting corrections.

Default: `false`

`pricingCurrency`

pricingCurrency

 (Required) 

The currency the transaction used to charge the customer. For more information, see pricingCurrency.

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

The net amount the customer was charged, accurate to the current report, that you state in milli-units of the reporting currency. This amount excludes tax, and accounts for all refunds and restatements. For more information, see netAmountTaxExclusive.

`taxAmount`

taxAmount

 (Required) 

The amount the customer paid in taxes, that you state in milli-units of the reporting currency. For more information, see taxAmount.

`taxCountry`

taxCountry

 (Required) 

The country code of the country for which taxes were paid on the purchase. For more information, see taxCountry.

`productIdentifier`

productIdentifier

 (Required) 

A string that uniquely identifies the product.

`quantity`

quantity

 (Required) 

The quantity of the product the customer purchased.

`eventType`

eventType

 (Required) 

Use `BUY`. (To report refunds or subscription-related transactions, use RefundLineItem or SubscriptionBuyLineItem line items instead.)

`productType`

productType

 (Required) 

Use `ONE_TIME_BUY`. (To report a subscription-related transaction, use a SubscriptionBuyLineItem instead.)

## Mentioned in 

Reporting tokens with transactions

Reporting corrections

## Discussion

Use a `OneTimeBuyLineItem` to report a one-time charge transaction, or a correction to a one-time charge transaction that you previously submitted.

Each line-item object represents one transaction. Other types of line-item objects include:

- SubscriptionBuyLineItem, for reporting subscription-related transactions

- RefundLineItem, for reporting refunds

Include the line-item objects in the `lineItems` array of an ExternalPurchaseReport object. To send the report, include the ExternalPurchaseReport object in a request to the Send External Purchase Report endpoint.

For more information, see Reporting tokens with transactions and Reporting corrections.

## See Also

### External purchase report transactions

Reporting tokens with transactions

Create reports for external purchase tokens that result in completed transactions, including one-time charges, subscriptions and renewals, and refunds.

Reporting corrections

Submit a report with corrections if you find errors in, or have adjustments to, a successfully submitted transaction.

object RefundLineItem

The line item that indicates a refund transaction.

object SubscriptionBuyLineItem

The line item that indicates a subscription-related event or transaction.

Line item fields

Properties that describe a single transaction or correction in an external purchase report.

