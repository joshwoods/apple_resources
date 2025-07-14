

- WebKit
- WKDownload
-  WKDownload.RedirectPolicy 

Enumeration

# WKDownload.RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
enum RedirectPolicy
```

## Topics

### Constants

case allow

Allow a redirect to proceed.

case cancel

Cancel the redirect action.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the download

var delegate: (any WKDownloadDelegate)?

An object you use to track download progress and handle redirects, authentication challenges, and failures.

func cancel(((Data?) -> Void)?)

Cancels the download, and optionally captures data so that you can resume the download later.

