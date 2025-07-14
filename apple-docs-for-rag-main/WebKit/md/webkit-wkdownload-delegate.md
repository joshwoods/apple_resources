

- WebKit
- WKDownload
-  delegate 

Instance Property

# delegate

An object you use to track download progress and handle redirects, authentication challenges, and failures.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
weak var delegate: (any WKDownloadDelegate)? { get set }
```

## See Also

### Managing the download

func cancel(((Data?) -> Void)?)

Cancels the download, and optionally captures data so that you can resume the download later.

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

