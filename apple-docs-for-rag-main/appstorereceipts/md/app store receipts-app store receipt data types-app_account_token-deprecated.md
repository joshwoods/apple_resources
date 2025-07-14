

- App Store Receipts
- App Store receipt data types
-  app_account_token Deprecated

Type

# app_account_token

The UUID that an app optionally generates to map a customer’s in-app purchase with its resulting App Store transaction.

App Store Receipts 1.5–1.7Deprecated

``` source
string app_account_token
```

## Discussion

When a customer initiates an in-app purchase, you can optionally generate an appAccountToken(_:) and send it to the App Store. The App Store returns the same value in appAccountToken in the transaction information after the customer completes the purchase.

If you’re using the Original API for In-App Purchase and provide a UUID in the applicationUsername property, then the `app_account_token` field contains that value.

## See Also

### Transaction identifiers

type original_transaction_id

The transaction identifier of the original purchase.

Deprecated

type transaction_id

A unique identifier for a transaction, such as a purchase, restore, or renewal.

Deprecated

