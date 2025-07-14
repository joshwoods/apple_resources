

- External Purchase Server API
-  ExternalPurchaseReport 

Object

# ExternalPurchaseReport

The contents of an external purchase report for a single token.

External Purchase Server API 1.0.0+

``` source
object ExternalPurchaseReport
```

## Properties

`requestIdentifier`

requestIdentifier

 (Required) 

A UUID that you generate to uniquely identify the report.

`externalPurchaseId`

externalPurchaseId

 (Required) 

The unique identifier of the external purchase token for which you submit the report.

`status`

status

 (Required) 

The status of the token that determines the information the report contains.

`lineItems`

`[*]`

An array of line items that describe transactions or events associated with the token identified by the `externalPurchaseId`.

Possible types: OneTimeBuyLineItem`, `SubscriptionBuyLineItem`, `RefundLineItem

## Mentioned in 

Reporting tokens with transactions

Reporting unrecognized tokens and tokens without transactions

Reporting corrections

## Discussion

This object is the request body for the Send External Purchase Report endpoint. Populate this object with data about a single external purchase token that you’re reporting, including its transactions. The Retrieve External Purchase Report endpoint also returns this object when you request a report you previously successfully submitted.

The `requestIdentifier` field identifies the report. Generate a UUID for each report you send.

Tip

Store the requestIdentifier value in your records with the external purchase token to identify your reports.

The externalPurchaseId field is the token’s identifier. To get that value, decode the external purchase token you receive in your app or on your website. For more information, see: Receiving and decoding external purchase tokens.

The status field represents the token’s status, which determines the report’s contents and whether it includes a `lineItems` array. The status value determines the three types of reports:

- A `LINE_ITEM` status for a report with transactions that you list in the `lineItems` array. Use this status when a token has associated transactions, and to send corrections to previously submitted line items. For more information, see Reporting tokens with transactions.

- A `NO_LINE_ITEM` status for a report of a token that didn’t result in any successful transactions. Don’t include `lineItems` in the request with this status. For more information, see: Reporting unrecognized tokens and tokens without transactions

- An `UNRECOGNIZED_TOKEN` status for a report of a token you receive in an App Store Server Notification, but that you don’t have recorded in your system. Don’t include `lineItems` in the request with this status. For more information, see Reporting unrecognized tokens and tokens without transactions

You can also submit corrections to restate line items, or retract a previous submission. For more information, see Reporting corrections.

A line item represents each transaction for the token identified by the `externalPurchaseId`. There are three types of line items:

- OneTimeBuyLineItem, for one-time charges

- RefundLineItem, for refunds

- SubscriptionBuyLineItem, for auto-renewable subscription events and transactions

Include as many line items as there are transactions that apply to the token. If your system completes new transactions after you successfully submit a report for a token, send a new report for the token with the new transactions.

## Topics

### Data types

type requestIdentifier

A UUID that uniquely identifies an external purchase report.

type externalPurchaseId

The unique identifier of an external purchase token.

type status

A string value that represents the status of the token and the contents of the external purchase report.

## See Also

### External purchase reporting

Send External Purchase Report

Report required information about external purchase tokens and associated transactions.

object SendReportSuccessResponse

A response that contains the request identifier and indicates the server successfully received your external purchase report.

object SendReportErrorResponse

An error response that indicates your external purchase report didn’t succeed, including error details for the line items in your report.

