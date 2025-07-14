

- App Store Receipts
-  responseBody Deprecated

Object

# responseBody

The JSON data that returns in the response from the App Store.

App Store Receipts 1.0–1.7Deprecated

Deprecated

The verifyReceipt endpoint is deprecated.

## Properties

`environment`

`string`

Deprecated 

The environment the system generates the receipt for.

Possible Values: `Sandbox, Production`

`is_retryable`

`boolean`

Deprecated 

An indicator when an error occurs during the request. A value of `1` indicates a temporary issue; retry validation for this receipt at a later time. A value of `0` indicates an unresolvable issue; don’t retry validation for this receipt. This is applicable only to status codes `21100–21199`.

`latest_receipt`

`byte`

Deprecated 

The latest Base64-encoded app receipt. This only returns for receipts that contain auto-renewable subscriptions.

`latest_receipt_info`

`[`responseBody.Latest_receipt_info`]`

Deprecated 

An array that contains all in-app purchase transactions. This excludes transactions for consumable products that your app marks as finished.

`pending_renewal_info`

`[`responseBody.Pending_renewal_info`]`

Deprecated 

In the JSON file, an array where each element contains the pending renewal information for each auto-renewable subscription the `product_id` identifies. This only returns for app receipts that contain auto-renewable subscriptions.

`receipt`

responseBody.Receipt

Deprecated 

A JSON representation of the receipt that you send for verification.

`status`

status

Deprecated 

Either `0` if the receipt is valid, or a status code if there’s an error. The status code reflects the status of the app receipt as a whole. See status for possible status codes and descriptions.

## Discussion

The verifyReceipt endpoint returns this response.

## Topics

### Objects

object responseBody.Pending_renewal_info

An array of elements that refers to open or failed auto-renewable subscription renewals.

object responseBody.Latest_receipt_info

An array that contains all in-app purchase transactions.

object responseBody.Receipt

The decoded version of the encoded receipt data that you send with the request to the App Store.

## See Also

### Deprecated

`verifyReceipt`

Send a receipt to the App Store for verification.

Deprecated

object requestBody

The JSON contents you submit with the request to the App Store.

Deprecated

object error

Error information that returns in the response body when a request isn’t successful.

Deprecated

