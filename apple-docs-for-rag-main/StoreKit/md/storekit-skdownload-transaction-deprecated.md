

- StoreKit
- SKDownload
-  transaction Deprecated

Instance Property

# transaction

The transaction associated with the downloadable file.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var transaction: SKPaymentTransaction { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

A download object is always associated with a payment transaction. The download object may only be queued after payment is processed and before the transaction is finished.

## See Also

### Getting Content Information

var expectedContentLength: Int64

The length of the downloadable content, in bytes.

Deprecated

var contentIdentifier: String

A string that uniquely identifies the downloadable content.

Deprecated

var contentVersion: String

A string that identifies which version of the content is available for download.

Deprecated

var contentLength: Int64

The length of the downloadable content, in bytes.

Deprecated

