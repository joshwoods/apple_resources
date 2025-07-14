

- External Purchase Server API
-  Reporting unrecognized tokens and tokens without transactions 

Article

# Reporting unrecognized tokens and tokens without transactions

Create reports for external purchase tokens that didn’t result in completed transactions, or tokens that you learn of from an App Store server notification.

## Overview

If a customer doesn’t successfully complete an external purchase, you must still report the token, even if it has no transaction. App Store Server Notifications V2 notifies you of external purchase tokens you haven’t yet reported, 10 days after the system created the token. You need to report the token, including when your system doesn’t have a record of the token.

Send a request to the Send External Purchase Report endpoint to report all external purchase tokens. Add the following information in the ExternalPurchaseReport request body:

- Supply a requestIdentifier, to uniquely identify the report.

- Provide the externalPurchaseId of the token you’re reporting.

Then, specify the type of report in the status field:

- Use `NO_LINE_ITEM` when the external purchase token doesn’t have any associated transactions.

- Use `UNRECOGNIZED_TOKEN` when you receive an App Store server notification with a external purchase token your system doesn’t recognize.

Don’t provide a `lineItems` field in the request body when using either of these status values.

### Report a token without a completed transaction

Use the `NO_LINE_ITEM` status to report an external purchase token that didn’t result in any completed transactions. The following example shows the `ExternalPurchaseReport` request body for a token without any associated transactions:

```
```

### Report an unrecognized token

Apple sends notifications to your App Store Server Notifications V2 endpoint for external purchase tokens that remain unreported after 10 days. The notification has a notificationType of `EXTERNAL_PURCHASE_TOKEN` and a subtype of `UNREPORTED`. It provides the token’s externalPurchaseId in the externalPurchaseToken field of notification’s payload.

Compare the `externalPurchaseId` to the tokens in your system. If your system doesn’t have a record of a matching token, use the `UNRECOGNIZED_TOKEN` status to send a report to Apple. The following example shows the ExternalPurchaseReport request body for an unrecognized token:

```
```

