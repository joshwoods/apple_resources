

- WebKit
- WKDownloadDelegate
-  download(\_:didFailWithError:resumeData:) 

Instance Method

# download(\_:didFailWithError:resumeData:)

Tells the delegate that the download failed, with error information and data you can use to restart the download.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
optional func download(
    _ download: WKDownload,
    didFailWithError error: any Error,
    resumeData: Data?
)
```

## Parameters 

`download`  

The download that failed.

`error`  

An error describing what caused the download to fail.

`resumeData`  

A data object you use to restart the download.

## Discussion

To restart a failed download, call resumeDownload(fromResumeData:completionHandler:) with `resumeData`.

## See Also

### Tracking Download Progress

func download(WKDownload, decideDestinationUsing: URLResponse, suggestedFilename: String, completionHandler: (URL?) -> Void)

Asks the delegate to provide a file destination where the system should write the download data.

**Required**

func downloadDidFinish(WKDownload)

Tells the delegate that the download finished.

