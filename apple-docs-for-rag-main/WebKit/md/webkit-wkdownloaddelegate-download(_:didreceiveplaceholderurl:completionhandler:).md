

- WebKit
- WKDownloadDelegate
-  download(\_:didReceivePlaceholderURL:completionHandler:) 

Instance Method

# download(\_:didReceivePlaceholderURL:completionHandler:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 11.3+visionOS 2.2+

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    didReceivePlaceholderURL url: URL,
    completionHandler: @escaping @MainActor () -> Void
)
```

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    didReceivePlaceholderURL url: URL
) async
```

