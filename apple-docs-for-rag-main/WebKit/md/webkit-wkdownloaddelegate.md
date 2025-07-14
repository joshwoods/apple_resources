

- WebKit
-  WKDownloadDelegate 

Protocol

# WKDownloadDelegate

A protocol you implement to track download progress and handle redirects, authentication challenges, and failures.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
@MainActor
protocol WKDownloadDelegate : NSObjectProtocol
```

## Topics

### Tracking Download Progress

func download(WKDownload, decideDestinationUsing: URLResponse, suggestedFilename: String, completionHandler: (URL?) -> Void)

Asks the delegate to provide a file destination where the system should write the download data.

**Required**

func downloadDidFinish(WKDownload)

Tells the delegate that the download finished.

func download(WKDownload, didFailWithError: any Error, resumeData: Data?)

Tells the delegate that the download failed, with error information and data you can use to restart the download.

### Responding to Authorization Challenges

func download(WKDownload, didReceive: URLAuthenticationChallenge, completionHandler: (URLSession.AuthChallengeDisposition, URLCredential?) -> Void)

Asks the delegate to respond to an authentication challenge.

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

### Responding to Redirects

func download(WKDownload, willPerformHTTPRedirection: HTTPURLResponse, newRequest: URLRequest, decisionHandler: (WKDownload.RedirectPolicy) -> Void)

Asks the delegate to respond to the download’s redirect response.

enum RedirectPolicy

An enumeration with cases that indicate whether to proceed with a redirect.

### Instance Methods

func download(WKDownload, decidePlaceholderPolicy: (WKDownload.PlaceholderPolicy, URL?) -> Void)

func download(WKDownload, didReceiveFinalURL: URL)

func download(WKDownload, didReceivePlaceholderURL: URL, completionHandler: () -> Void)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Downloads

class WKDownload

An object that represents the download of a web resource.

