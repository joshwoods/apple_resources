

- StoreKit
- SKDownload
-  error Deprecated

Instance Property

# error

The error that prevented the content from being downloaded.

iOS 6.0–16.0DeprecatediPadOS 6.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 6.2–9.0Deprecated

``` source
var error: (any Error)? { get }
```

Deprecated

Hosted content is no longer supported

## Mentioned in 

Unlocking purchased content

## Discussion

The value of this property is valid only when the downloadState property is set to SKDownloadState.failed.

## See Also

### Accessing a Completed Download

var contentURL: URL?

The local location of the downloaded file.

Deprecated

