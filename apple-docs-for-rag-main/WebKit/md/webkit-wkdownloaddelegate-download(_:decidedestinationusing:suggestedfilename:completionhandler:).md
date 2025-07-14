

- WebKit
- WKDownloadDelegate
-  download(\_:decideDestinationUsing:suggestedFilename:completionHandler:) 

Instance Method

# download(\_:decideDestinationUsing:suggestedFilename:completionHandler:)

Asks the delegate to provide a file destination where the system should write the download data.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
func download(
    _ download: WKDownload,
    decideDestinationUsing response: URLResponse,
    suggestedFilename: String,
    completionHandler: @escaping @MainActor (URL?) -> Void
)
```

``` source
@MainActor
func download(
    _ download: WKDownload,
    decideDestinationUsing response: URLResponse,
    suggestedFilename: String
) async -> URL?
```

**Required**

## Parameters 

`download`  

The download that needs a file destination where the systems should write the download data.

`response`  

A response from the server for an HTTP request, or a synthesized response for a blob download.

`suggestedFilename`  

A string with a filename suggestion to use in creating the file destination.

`completionHandler`  

A closure you invoke with a destination file URL to begin the download, or `nil` to cancel the download.

## Discussion

The suggested filename can come from the response or from the web content.

The destination file URL must meet the following requirements:

- It’s a file that doesn’t exist.

- It’s in a directory that exists.

- It’s in a directory that WebKit can write to.

## See Also

### Tracking Download Progress

func downloadDidFinish(WKDownload)

Tells the delegate that the download finished.

func download(WKDownload, didFailWithError: any Error, resumeData: Data?)

Tells the delegate that the download failed, with error information and data you can use to restart the download.

