

- StoreKit
- SKReceiptRefreshRequest
-  init(receiptProperties:) Deprecated

Initializer

# init(receiptProperties:)

Creates a receipt refresh request with optional properties.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
init(receiptProperties properties: [String : Any]?)
```

Deprecated

Use Transaction.all and AppTransaction.shared

## Parameters 

`properties`  

In the test environment, the properties that the new receipt is to have. For keys, see Receipt Properties and Keys.

In the production environment, set this parameter to `nil`.

## Return Value

The initialized request.

## Mentioned in 

Restoring purchased products

## Discussion

In the sandbox environment, you can initialize a receipt with any combination of properties to test the state transitions related to Volume Purchase Plan receipts. Set the `properties` when you call this initializer.

