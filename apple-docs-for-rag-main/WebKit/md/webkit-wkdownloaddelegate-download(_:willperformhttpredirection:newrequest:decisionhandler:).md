

- WebKit
- WKDownloadDelegate
-  download(\_:willPerformHTTPRedirection:newRequest:decisionHandler:) 

Instance Method

# download(\_:willPerformHTTPRedirection:newRequest:decisionHandler:)

Asks the delegate to respond to the download’s redirect response.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    willPerformHTTPRedirection response: HTTPURLResponse,
    newRequest request: URLRequest,
    decisionHandler: @escaping @MainActor (WKDownload.RedirectPolicy) -> Void
)
```

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    decidedPolicyForHTTPRedirection response: HTTPURLResponse,
    newRequest request: URLRequest
) async -> WKDownload.RedirectPolicy
```

## Parameters 

`download`  

The download that receives the redirect response.

`response`  

The redirect response.

`request`  

The new request the web view sends as a result of the redirect response.

`decisionHandler`  

A closure you must invoke, providing a download redirect policy that indicates whether to proceed with the redirect.

## Discussion

Determine whether to proceed with the redirect. Then invoke the decisionHandler closure, providing a download redirect policy that indicates whether to proceed with the redirect.

If you don’t implement this method, the web view proceeds with all redirects.

## See Also

### Responding to Redirects

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

