

- WebKit
- WKWebView
-  startDownload(using:completionHandler:) 

Instance Method

# startDownload(using:completionHandler:)

Starts to download the resource at the URL in the request.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
func startDownload(
    using request: URLRequest,
    completionHandler: @escaping @MainActor (WKDownload) -> Void
)
```

``` source
@MainActor
func startDownload(using request: URLRequest) async -> WKDownload
```

## Parameters 

`request`  

An object that encapsulates a URL and other parameters that you need to download a resource from a webpage.

`completionHandler`  

A closure the system executes when it has started to download the resource.

## Discussion

To receive progress updates, set the delegate of the download object in the completion handler.

## See Also

### Managing downloads

func resumeDownload(fromResumeData: Data, completionHandler: (WKDownload) -> Void)

Resumes a failed or canceled download.

