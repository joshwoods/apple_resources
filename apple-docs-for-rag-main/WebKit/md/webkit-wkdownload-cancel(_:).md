

- WebKit
- WKDownload
-  cancel(\_:) 

Instance Method

# cancel(\_:)

Cancels the download, and optionally captures data so that you can resume the download later.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
func cancel(_ completionHandler: (@MainActor (Data?) -> Void)? = nil)
```

``` source
@MainActor
func cancel() async -> Data?
```

## Parameters 

`completionHandler`  

A closure you provide to capture and store data so that you can resume the download later.

## Discussion

Concurrency Note

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func cancel() async -> Data?
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Managing the download

var delegate: (any WKDownloadDelegate)?

An object you use to track download progress and handle redirects, authentication challenges, and failures.

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

