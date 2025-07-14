

- External Purchase Server API
-  Reporting corrections 

Article

# Reporting corrections

Submit a report with corrections if you find errors in, or have adjustments to, a successfully submitted transaction.

## Overview

If you successfully submit a report to the Send External Purchase Report endpoint that you later find to be incorrect, you must correct your submission. To send a correction, fill out the ExternalPurchaseReport request body with a new requestIdentifier and the corrections, and call the Send External Purchase Report endpoint. Send corrected reports promptly.

There are two types of corrections:

- A correction to transaction data in a line item. In this type of correction, you restate the entire line item with corrected data. Apple uses only the most recent submission for the line item.

- A retraction of a line item you previously sent. In this type of correction, you indicate that you erroneously sent the line item, and aren’t including the erroneously-submitted amounts in transaction calculations. Be sure to update the netAmountTaxExclusive field so it represents the correct net amount, tax exclusive, of the transaction.

Important

The netAmountTaxExclusive must represent the correct net amount (excluding taxes) for the transaction, including in line items that are corrections.

### Correct data in a line item

To submit a line item with corrections, use the line item’s original lineItemId and include the restatement flag set to `true`. Make corrections to any type of line item: OneTimeBuyLineItem, SubscriptionBuyLineItem, and RefundLineItem.

Important

Restated line items overwrite the originally reported line item. Include all the data in the line item — even fields that are the same as the previous version.

Apple uses only the most recent version of the line item.

### Retract an erroneously submitted line item

If you submitted a line item in error and want Apple to ignore it, use the same lineItemId as in the original submission. Set both the restatement and erroneouslySubmitted fields to `true`. (You may undo this action by submitting the line item again, with restatement set to `true`, and erroneouslySubmitted set to false.) Be sure to include all of the original line item data fields, and recalculate the netAmountTaxExclusive field to correctly represent the net amount with the erroneously submitted line item accounted for.

Successfully submitting a line item with the `erroneouslySubmitted` flag is an effective “undo” of the original line item.

## See Also

### External purchase report transactions

Reporting tokens with transactions

Create reports for external purchase tokens that result in completed transactions, including one-time charges, subscriptions and renewals, and refunds.

object OneTimeBuyLineItem

The line item that indicates a one-time charge transaction.

object RefundLineItem

The line item that indicates a refund transaction.

object SubscriptionBuyLineItem

The line item that indicates a subscription-related event or transaction.

Line item fields

Properties that describe a single transaction or correction in an external purchase report.

