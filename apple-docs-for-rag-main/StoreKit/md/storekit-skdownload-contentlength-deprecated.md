

- StoreKit
- SKDownload
-  contentLength Deprecated

Instance Property

# contentLength

The length of the downloadable content, in bytes.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.0–13.0DeprecatedmacOS 10.8–10.15DeprecatedtvOS 9.0–13.0Deprecated

**iOS, iPadOS, Mac Catalyst, tvOS**

``` source
var contentLength: Int64 { get }
```

**macOS**

``` source
@NSCopying
var contentLength: NSNumber { get }
```

Deprecated

Use expectedContentLength instead.

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

var transaction: SKPaymentTransaction

The transaction associated with the downloadable file.

Deprecated

