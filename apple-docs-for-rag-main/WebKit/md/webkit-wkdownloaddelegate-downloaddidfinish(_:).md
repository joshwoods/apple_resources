

- WebKit
- WKDownloadDelegate
-  downloadDidFinish(\_:) 

Instance Method

# downloadDidFinish(\_:)

Tells the delegate that the download finished.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
optional func downloadDidFinish(_ download: WKDownload)
```

## Parameters 

`download`  

The download that finished.

## See Also

### Tracking Download Progress

func download(WKDownload, decideDestinationUsing: URLResponse, suggestedFilename: String, completionHandler: (URL?) -> Void)

Asks the delegate to provide a file destination where the system should write the download data.

**Required**

func download(WKDownload, didFailWithError: any Error, resumeData: Data?)

Tells the delegate that the download failed, with error information and data you can use to restart the download.

