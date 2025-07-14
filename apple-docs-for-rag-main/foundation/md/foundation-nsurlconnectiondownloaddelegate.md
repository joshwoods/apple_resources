

- Foundation
-  NSURLConnectionDownloadDelegate 

Protocol

# NSURLConnectionDownloadDelegate

A protocol that delegates of a URL connection created with Newsstand Kit implement to receive data associated with a download.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSURLConnectionDownloadDelegate : NSURLConnectionDelegate
```

## Overview

The `NSURLConnectionDownloadDelegate` protocol describes methods that should be implemented by the delegate of instances of `NSURLConnection` created using Newsstand Kit’s `download(with:)` method. The methods in this protocol provide progress information about the download of a URL asset and, when downloading concludes, provide a file URL where the downloaded file can be accessed.

In addition to the methods described in this protocol, an `NSURLConnection` delegate should also implement the methods described in the NSURLConnectionDelegate protocol.

Note

If you are using `NSURLConnection` directly, your delegate class should instead implement the methods defined in the NSURLConnectionDataDelegate protocol.

## Topics

### Managing Downloads of URL Assets

func connection(NSURLConnection, didWriteData: Int64, totalBytesWritten: Int64, expectedTotalBytes: Int64)

Sent to the delegate to deliver progress information for a download of a URL asset to a destination file.

func connectionDidResumeDownloading(NSURLConnection, totalBytesWritten: Int64, expectedTotalBytes: Int64)

Sent to the delegate when an URL connection resumes downloading a URL asset that was earlier suspended.

func connectionDidFinishDownloading(NSURLConnection, destinationURL: URL)

Sent to the delegate when the URL connection has successfully downloaded the URL asset to a destination file.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- NSURLConnectionDelegate

## See Also

### URL Connection

class NSURLConnection

An object that enables you to start and stop URL requests.

protocol NSURLConnectionDelegate

A protocol that delegates of a URL connection implement to receive status about and provide feedback to the connection object.

protocol NSURLConnectionDataDelegate

A protocol that most delegates of a URL connection implement to receive data associated with the connection.

