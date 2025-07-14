

- StoreKit
- SKDownload
-  contentURL Deprecated

Instance Property

# contentURL

The local location of the downloaded file.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var contentURL: URL? { get }
```

Deprecated

Hosted content is no longer supported

## Mentioned in 

Unlocking purchased content

## Discussion

The value of this property is valid only when the downloadState property is set to SKDownloadState.finished. The URL becomes invalid after the transaction object associated with the download is finalized.

## See Also

### Accessing a Completed Download

var error: (any Error)?

The error that prevented the content from being downloaded.

Deprecated

