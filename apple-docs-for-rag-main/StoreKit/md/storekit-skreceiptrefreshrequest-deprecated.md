

- StoreKit
-  SKReceiptRefreshRequest Deprecated

Class

# SKReceiptRefreshRequest

A request to the App Store to get the app receipt, which represents the customer’s transactions with your app.

iOS 7.0–18.0DeprecatediPadOS 7.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOSDeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
class SKReceiptRefreshRequest
```

Deprecated

Use Transaction.all and AppTransaction.shared

## Mentioned in 

Choosing a receipt validation technique

Restoring purchased products

Validating receipts with the App Store

## Overview

Note

The receipt isn’t necessary if you use AppTransaction to validate the app download, or Transaction to validate in-app purchases. Only use the receipt if your app uses the Original API for In-App Purchase, or needs the receipt to validate the app download because it can’t use AppTransaction.

Use this API to request a new app receipt from the App Store if the receipt is invalid or missing from its expected location, appStoreReceiptURL. To request the receipt using the SKReceiptRefreshRequest object, you initialize it, attach a delegate, and then call the request’s start() method.

Important

The receipt refresh request displays a system prompt that asks users to authenticate with their App Store credentials. For a better user experience, initiate the request after an explicit user action, like tapping or clicking a button.

When the request completes successfully, your delegate receives an SKReceiptRefreshRequest object in its requestDidFinish(_:) method. Locate the app receipt using the appStoreReceiptURL property. For information about validating the receipt, see Choosing a receipt validation technique.

If the request fails and calls your delegate’s request(_:didFailWithError:) method, your app needs to release the request and not attempt to call it a second time. Requests can fail when a user doesn’t authenticate or chooses to cancel the request. Without a validated receipt, assume the user doesn’t have access to premium content.

In the sandbox environment, you can initialize a receipt with any combination of properties for testing when you call init(receiptProperties:).

### Use alternative techniques

There are times when using SKReceiptRefreshRequest isn’t necessary, so avoid doing so, such as in the following scenarios:

- If the receipt is valid, but may be missing transactions, use restoreCompletedTransactions() instead. For example, the receipt may be missing a transaction if a person purchases a new subscription on another device.

- In the sandbox environment, before the tester completes their first in-app purchase. Receipts are initially absent in the sandbox environment for iOS and iPadOS apps. For more information, see appStoreReceiptURL.

## Topics

### Initializing Receipt Refresh Requests

init(receiptProperties: [String : Any]?)

Creates a receipt refresh request with optional properties.

### Receipt Properties and Keys

var receiptProperties: [String : Any]?

The properties of the receipt.

let SKReceiptPropertyIsExpired: String

A key with a value that indicates whether the receipt is in an expired state.

let SKReceiptPropertyIsRevoked: String

A key with a value that indicates whether the receipt is in a revoked state.

let SKReceiptPropertyIsVolumePurchase: String

A key with a value that indicates whether the receipt is a Volume Purchase Plan receipt.

## Relationships

### Inherits From

- SKRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Purchase validation

Choosing a receipt validation technique

Select the type of receipt validation, on the device or on your server, that works for your app.

Validating receipts with the App Store

Verify transactions with the App Store on a secure server.

var appStoreReceiptURL: URL?

The file URL for the bundle’s App Store receipt.

