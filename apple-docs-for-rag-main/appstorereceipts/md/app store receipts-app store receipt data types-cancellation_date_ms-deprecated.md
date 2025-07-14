

- App Store Receipts
- App Store receipt data types
-  cancellation_date_ms Deprecated

Type

# cancellation_date_ms

The time and date that the App Store refunds a transaction or revokes it from Family Sharing.

App Store Receipts 1.0–1.7Deprecated

``` source
string cancellation_date_ms
```

## Discussion

This field is returned in the JSON response, in the responseBody.Latest_receipt_info and responseBody.Receipt.In_app arrays.

This field represents the time and date the App Store refunded a transaction or revoked it from family sharing, in UNIX epoch time format, in milliseconds. This field is only present for purchases that Apple refunded or revoked. Use this time format for processing dates.

A canceled in-app purchase remains in the receipt indefinitely. This value is present only if the refund or revocation was for a non-consumable product, an auto-renewable subscription, or a non-renewing subscription.

Use this value to determine whether to stop providing the content associated with the purchase.

## See Also

### Dates and intent

type expiration_intent

The reason a subscription expires.

Deprecated

type expires_date_ms

The time, in milliseconds, a subscription expires or renews.

Deprecated

