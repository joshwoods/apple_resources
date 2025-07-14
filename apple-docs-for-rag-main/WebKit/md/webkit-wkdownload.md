

- WebKit
-  WKDownload 

Class

# WKDownload

An object that represents the download of a web resource.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
class WKDownload
```

## Topics

### Managing the download

var delegate: (any WKDownloadDelegate)?

An object you use to track download progress and handle redirects, authentication challenges, and failures.

func cancel(((Data?) -> Void)?)

Cancels the download, and optionally captures data so that you can resume the download later.

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

### Inspecting the download

var originalRequest: URLRequest?

An object that represents the request that initiated the download.

var webView: WKWebView?

The web view where the download initiated.

### Instance Properties

var isUserInitiated: Bool

var originatingFrame: WKFrameInfo

### Enumerations

enum PlaceholderPolicy

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- ProgressReporting
- Sendable

## See Also

### Downloads

protocol WKDownloadDelegate

A protocol you implement to track download progress and handle redirects, authentication challenges, and failures.

