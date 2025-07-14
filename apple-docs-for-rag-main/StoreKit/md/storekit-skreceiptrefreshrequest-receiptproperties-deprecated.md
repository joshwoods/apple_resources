

- StoreKit
- SKReceiptRefreshRequest
-  receiptProperties Deprecated

Instance Property

# receiptProperties

The properties of the receipt.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
var receiptProperties: [String : Any]? { get }
```

Deprecated

Use Transaction.all and AppTransaction.shared

## Discussion

Receipt properties include SKReceiptPropertyIsExpired, SKReceiptPropertyIsRevoked, and SKReceiptPropertyIsVolumePurchase.

## See Also

### Receipt Properties and Keys

let SKReceiptPropertyIsExpired: String

A key with a value that indicates whether the receipt is in an expired state.

Deprecated

let SKReceiptPropertyIsRevoked: String

A key with a value that indicates whether the receipt is in a revoked state.

Deprecated

let SKReceiptPropertyIsVolumePurchase: String

A key with a value that indicates whether the receipt is a Volume Purchase Plan receipt.

Deprecated

