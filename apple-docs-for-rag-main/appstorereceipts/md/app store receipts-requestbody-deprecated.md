

- App Store Receipts
-  requestBody Deprecated

Object

# requestBody

The JSON contents you submit with the request to the App Store.

App Store Receipts 1.0–1.7Deprecated

Deprecated

The verifyReceipt endpoint is deprecated.

## Properties

`receipt-data`

`byte`

Deprecated   (Required) 

The Base64-encoded receipt data.

`password`

`string`

Deprecated 

Your app’s shared secret, which is a hexadecimal string. The password is required for receipts that include subscriptions, and strongly recommended otherwise. For more information about the shared secret, see Generate a shared secret to verify receipts.

`exclude-old-transactions`

`boolean`

Deprecated 

Set this value to `true` for the response to include only the latest renewal transaction for any subscriptions. Use this field only for app receipts that contain auto-renewable subscriptions.

## Discussion

To receive a decoded receipt for validation, send a request with the encoded receipt data and app password to the App Store. For receipts that contain auto-renewable subscriptions, optionally include an exclusion flag. Send this JSON data using the HTTP POST request method.

## See Also

### Deprecated

`verifyReceipt`

Send a receipt to the App Store for verification.

Deprecated

object responseBody

The JSON data that returns in the response from the App Store.

Deprecated

object error

Error information that returns in the response body when a request isn’t successful.

Deprecated

