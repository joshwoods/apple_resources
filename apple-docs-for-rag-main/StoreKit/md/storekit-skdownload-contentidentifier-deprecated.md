

- StoreKit
- SKDownload
-  contentIdentifier Deprecated

Instance Property

# contentIdentifier

A string that uniquely identifies the downloadable content.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var contentIdentifier: String { get }
```

Deprecated

Hosted content is no longer supported

## Discussion

Each piece of downloadable content associated with a product has its own unique identifier. The content identifier is specified in App Store Connect when you add the content.

## See Also

### Related Documentation

In-App Purchase Programming Guide

### Getting Content Information

var expectedContentLength: Int64

The length of the downloadable content, in bytes.

Deprecated

var contentVersion: String

A string that identifies which version of the content is available for download.

Deprecated

var transaction: SKPaymentTransaction

The transaction associated with the downloadable file.

Deprecated

var contentLength: Int64

The length of the downloadable content, in bytes.

Deprecated

