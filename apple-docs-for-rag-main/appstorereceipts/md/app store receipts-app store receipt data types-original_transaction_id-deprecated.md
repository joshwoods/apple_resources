

- App Store Receipts
- App Store receipt data types
-  original_transaction_id Deprecated

Type

# original_transaction_id

The transaction identifier of the original purchase.

App Store Receipts 1.0–1.7Deprecated

``` source
string original_transaction_id
```

## Discussion

This field is returned in the JSON response, in the responseBody.Pending_renewal_info, responseBody.Latest_receipt_info, and responseBody.Receipt.In_app arrays.

This value is identical to the transaction_id except when the user restores a purchase or renews a subscription. This value has the same format as the transaction’s `transactionIdentifier` property; however, the values may not be the same. For auto-renewable subscription transactions, this value also appears in the `pending_renewal_info` key of the JSON response.

You can use this value to:

- Match a transaction found in the receipt to a server-to-server notification event. For more information, see Enabling App Store Server Notifications.

- Manage auto-renewable subscriptions. Store this value, `product_id`, `expires_date_ms`, and `purchase_date_ms` for each transaction for each customer, as a best practice.

- Identify a subscription with the `product_id` in the `pending_renewal_info` section. Do not rely on the `original_transaction_id` value on its own. Treat this purchase as a new subscription when you see a new `original_transaction_id` value for a `product_id`.

- Differentiate a purchase transaction from a restore or a renewal transaction. In a purchase transaction, the `transaction_id` always matches the `original_transaction_id`. For subscriptions, it indicates the first subscription purchase. For a restore or renewal, the `transaction_id` does not match the `original_transaction_id`.

- Identify one or more renewals for the same subscription.

## See Also

### Transaction identifiers

type transaction_id

A unique identifier for a transaction, such as a purchase, restore, or renewal.

Deprecated

type app_account_token

The UUID that an app optionally generates to map a customer’s in-app purchase with its resulting App Store transaction.

Deprecated

