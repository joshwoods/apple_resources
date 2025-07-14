

- External Purchase Server API
-  SubscriptionBuyLineItem 

Object

# SubscriptionBuyLineItem

The line item that indicates a subscription-related event or transaction.

External Purchase Server API 1.0.0+

``` source
object SubscriptionBuyLineItem
```

## Properties

`lineItemId`

lineItemId

 (Required) 

A unique identifier for the transaction, that you determine. The value must be unique per app. Using UUIDs is recommended. Reuse a `lineItemId` only to submit a correction for a previously submitted line item.

`referenceLineItemId`

referenceLineItemId

The lineItemId of initial purchase transaction for the subscription.

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

`subscriptionEvent`

subscriptionEvent

 (Required) 

The subscription event the transaction represents, including a subscription start, a renewal, a change, or a payment. For more information, see subscriptionEvent.

`subscriptionStartDate`

subscriptionStartDate

 (Required) 

The UNIX date, in milliseconds, of the start of the subscription renewal period.

`subscriptionEndDate`

subscriptionEndDate

 (Required) 

The UNIX date, in milliseconds, of the end of the subscription renewal period.

`subscriptionDaysOfPaidService`

subscriptionDaysOfPaidService

 (Required) 

The total number of days of paid service for the subscription. For more information, see subscriptionDaysOfPaidService.

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

The net amount the customer was charged, accurate to the current line item, that you state in milli-units of the reporting currency. This amount excludes tax, and accounts for all refunds and restatements. For more information, see netAmountTaxExclusive.

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

A string that uniquely identifies the subscription product.

`quantity`

quantity

 (Required) 

The quantity of the product the customer purchased. For more information, see quantity.

`eventType`

eventType

 (Required) 

Use `BUY`. (To report a refund, use a RefundLineItem line item instead.)

`productType`

productType

 (Required) 

Use `SUBSCRIPTION`. (To report a one-time charge transaction, use a OneTimeBuyLineItem instead.)

## Mentioned in 

Reporting tokens with transactions

Reporting corrections

## Discussion

Use a `SubscriptionBuyLineItem` to report a subscription-related transaction or event, or a correction to the same.

Each line-item object represents one transaction. Other types of line-item objects include:

- OneTimeBuyLineItem, for reporting a one-time charge

- RefundLineItem, for reporting refunds

Include the line-item objects in the `lineItems` array of an ExternalPurchaseReport object. To send the report, include the ExternalPurchaseReport object in a request to the Send External Purchase Report endpoint.

Note

Identify a subscription using the lineItemId of the original subscription-start transaction. A line item for a subscription start has an eventType of `BUY` and a subscriptionEvent of `SUBSCRIPTION_START`.

For example, to report a renewal for a subscription, set the renewal transaction’s referenceLineItemId to the `lineItemId` of the subscription-start line item, and set the `subscriptionEvent` to `RENEWAL`.

For more information, see Reporting tokens with transactions and Reporting corrections.

## See Also

### External purchase report transactions

Reporting tokens with transactions

Create reports for external purchase tokens that result in completed transactions, including one-time charges, subscriptions and renewals, and refunds.

Reporting corrections

Submit a report with corrections if you find errors in, or have adjustments to, a successfully submitted transaction.

object OneTimeBuyLineItem

The line item that indicates a one-time charge transaction.

object RefundLineItem

The line item that indicates a refund transaction.

Line item fields

Properties that describe a single transaction or correction in an external purchase report.

