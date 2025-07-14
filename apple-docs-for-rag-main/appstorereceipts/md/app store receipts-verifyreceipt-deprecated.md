

- App Store Receipts
-  verifyReceipt Deprecated

Web Service Endpoint

# verifyReceipt

Send a receipt to the App Store for verification.

App Store Receipts 1.0–1.7Deprecated

Deprecated

The `verifyReceipt` endpoint is deprecated. To validate receipts on your server, follow the steps in Validating receipts on the device on your server. To validate in-app purchases on your server without using receipts, call the App Store Server API to get Apple-signed transaction and subscription information for your customers, or verify the AppTransaction and Transaction signed data that your app obtains. You can also get the same signed transaction and subscription information from the App Store Server Notifications V2 endpoint.

## URL

``` source
POST https://buy.itunes.apple.com/verifyReceipt
```

## Sandbox URL

``` source
POST https://sandbox.itunes.apple.com/verifyReceipt
```

## HTTP Body

requestBody

The JSON contents you submit with the request.

Content-Type: application/json

## Response Codes

` 200 ``OK`

responseBody

`OK`

Content-Type: application/json

## Discussion

Validating with the App Store requires a secure connection between your app and your server, as well as code on your server to validate the receipt with the App Store. Submit an HTTP POST request with the contents detailed in requestBody using the `verifyReceipt` endpoint to verify receipts with the App Store. Use the receipt fields in the responseBody to validate app and in-app purchases.

Your server must support the Transport Layer Security (TLS) protocol 1.2 or later to call this endpoint.

For more information about server-side receipt validation, see Validating receipts with the App Store.

### Use the sandbox URL for sandbox testing

The sandbox URL for verifying receipts is:

POST https://sandbox.itunes.apple.com/verifyReceipt

Important

As a best practice, always call the production URL `https://buy.itunes.apple.com/verifyReceipt` first and proceed to verify with the sandbox URL if you receive a `21007` status code. Following this approach ensures that you don’t have to switch between URLs while your app is in testing, in review by App Review, or live in the App Store.

### Find deprecation date in the HTTP header

The `verifyReceipt` endpoint is deprecated. The HTTP header includes the deprecation date, according to RFC 8594.

## See Also

### Deprecated

object requestBody

The JSON contents you submit with the request to the App Store.

Deprecated

object responseBody

The JSON data that returns in the response from the App Store.

Deprecated

object error

Error information that returns in the response body when a request isn’t successful.

Deprecated

