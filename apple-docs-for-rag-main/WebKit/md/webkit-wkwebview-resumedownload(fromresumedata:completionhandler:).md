

- WebKit
- WKWebView
-  resumeDownload(fromResumeData:completionHandler:) 

Instance Method

# resumeDownload(fromResumeData:completionHandler:)

Resumes a failed or canceled download.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
func resumeDownload(
    fromResumeData resumeData: Data,
    completionHandler: @escaping @MainActor (WKDownload) -> Void
)
```

``` source
@MainActor
func resumeDownload(fromResumeData resumeData: Data) async -> WKDownload
```

## Parameters 

`resumeData`  

An object with data that you use to resume a failed or canceled download.

`completionHandler`  

A closure the system executes when it has resumed a download.

## Discussion

To receive progress updates, set the delegate of the download object in the completion handler.

## See Also

### Managing downloads

func startDownload(using: URLRequest, completionHandler: (WKDownload) -> Void)

Starts to download the resource at the URL in the request.

