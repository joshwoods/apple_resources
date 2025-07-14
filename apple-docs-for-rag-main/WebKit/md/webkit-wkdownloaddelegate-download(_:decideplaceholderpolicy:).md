

- WebKit
- WKDownloadDelegate
-  download(\_:decidePlaceholderPolicy:) 

Instance Method

# download(\_:decidePlaceholderPolicy:)

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 11.3+visionOS 2.2+

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    decidePlaceholderPolicy completionHandler: @escaping @MainActor (WKDownload.PlaceholderPolicy, URL?) -> Void
)
```

``` source
@MainActor
optional func placeholderPolicy(forDownload download: WKDownload) async -> (WKDownload.PlaceholderPolicy, URL?)
```

