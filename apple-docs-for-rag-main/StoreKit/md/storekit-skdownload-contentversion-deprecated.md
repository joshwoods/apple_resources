

- StoreKit
- SKDownload
-  contentVersion Deprecated

Instance Property

# contentVersion

A string that identifies which version of the content is available for download.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var contentVersion: String { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

The version string must be formatted as a series of integers separated by periods.

## See Also

### Getting Content Information

var expectedContentLength: Int64

The length of the downloadable content, in bytes.

Deprecated

var contentIdentifier: String

A string that uniquely identifies the downloadable content.

Deprecated

var transaction: SKPaymentTransaction

The transaction associated with the downloadable file.

Deprecated

var contentLength: Int64

The length of the downloadable content, in bytes.

Deprecated

