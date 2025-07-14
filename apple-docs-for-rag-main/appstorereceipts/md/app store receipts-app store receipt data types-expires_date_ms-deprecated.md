

- App Store Receipts
- App Store receipt data types
-  expires_date_ms Deprecated

Type

# expires_date_ms

The time, in milliseconds, a subscription expires or renews.

App Store Receipts 1.0–1.7Deprecated

``` source
string expires_date_ms
```

## Discussion

This field is returned in the JSON response, in the responseBody.Latest_receipt_info and responseBody.Receipt.In_app arrays.

The time a subscription expires or when it will renew, in UNIX epoch time format, in milliseconds. Use this time format for processing dates.

You can use this date value to:

- Manage auto-renewable subscriptions. Store this value, `original_transaction_id`, `product_id`, and `purchase_date_ms` for each subscription, as a best practice.

- Identify the date the subscription renews or expires.

- Determine a user’s access to content or a service by comparing this date to the current date. After validating the latest receipt, continue providing service if the date is in the future. If the subscription expiration date for the latest renewal transaction has passed, the subscription has expired.

## See Also

### Dates and intent

type expiration_intent

The reason a subscription expires.

Deprecated

type cancellation_date_ms

The time and date that the App Store refunds a transaction or revokes it from Family Sharing.

Deprecated

