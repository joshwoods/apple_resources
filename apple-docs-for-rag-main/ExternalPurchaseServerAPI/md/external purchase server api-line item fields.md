

- External Purchase Server API
-  Line item fields 

API Collection

# Line item fields

Properties that describe a single transaction or correction in an external purchase report.

## Topics

### Identifying the line item

type lineItemId

A unique identifier for the line item, that you determine.

### Providing transaction info

type creationDate

The UNIX date, in milliseconds, that the customer authorized the transaction.

type eventType

The type of transaction the line item reports, whether it’s a buy or refund.

type referenceLineItemId

The line item identifier of another transaction, that the report references.

### Providing product info

type productIdentifier

A string that identifies the product.

type productType

The type of product in the transaction, whether it’s a one-time buy, or a subscription.

type quantity

The quantity of the product the customer purchased in a single transaction.

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

type pricingCurrency

The currency used in the transaction to bill or refund the customer.

type reportingCurrency

The currency the line item uses to report all amount values.

type exchangeRate

A decimal value that is the exchange rate you use to convert the pricing currency to the reporting currency, when the two currencies differ.

### Supplying subscription info

type subscriptionDaysOfPaidService

The total number of days of paid service for the subscription.

type subscriptionEndDate

The UNIX date, in milli-seconds, the subscription renewal cycle ends.

type subscriptionEvent

The event in the subscription’s life cycle that the transaction represents.

type subscriptionStartDate

The UNIX date, in milli-seconds, of the start of the subscription renewal period.

type referenceLineItemId

The line item identifier of another transaction, that the report references.

### Submitting corrections

type erroneouslySubmitted

A Boolean value that indicates whether a line item was submitted in error.

type restatement

A Boolean value that indicates a line item contains a correction.

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

object SubscriptionBuyLineItem

The line item that indicates a subscription-related event or transaction.

