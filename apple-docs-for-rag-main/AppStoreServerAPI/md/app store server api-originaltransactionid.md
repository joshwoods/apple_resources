

- App Store Server API
-  originalTransactionId 

Type

# originalTransactionId

The original transaction identifier of a purchase.

App Store Server API 1.0+

``` source
string originalTransactionId
```

## Mentioned in 

App Store Server API changelog

Extending the renewal date for auto-renewable subscriptions

## Discussion

The App Store generates an original transaction identifier when a customer makes a successful in-app purchase. Most App Store Server API endpoints accept an `originalTransactionId`.

There are several ways to obtain this value: from your app after a user makes a successful in-app purchase, from transaction information provided in App Store Server Notifications, or from App Store Receipts for apps that use the Original API for In-App Purchase.

To get the original transaction identifier from your app, use the originalID property of the Transaction object that represents the in-app purchase.

If you’ve enabled App Store Server Notifications, your server receives notifications for in-app purchase events that include the transaction information with the original transaction identifier. For more information, see responseBodyV2DecodedPayload.

If your app uses the Original API for In-App Purchase, the original transaction identifier is the transactionIdentifier property in the SKPaymentTransaction object. For restored purchases, the original transaction identifier is found in the transactionIdentifier of the original property. If you verify receipts using verifyReceipt, the original transaction identifier is the original_transaction_id value.

Use the value of the original transaction identifier that you get from your app, a notification, or a receipt as the value for originalTransactionId when you send requests to the App Store Server API.

Tip

If you maintain a database to manage your subscribers, save the original transaction identifier to uniquely identify auto-renewable subscriptions.

## See Also

### Response data types

type effectiveDate

The new subscription expiration date for a subscription-renewal extension.

type success

A Boolean value that indicates whether the subscription-renewal-date extension succeeded.

type webOrderLineItemId

The unique identifier of subscription-purchase events across devices, including renewals.

