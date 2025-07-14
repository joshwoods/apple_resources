

- Foundation
- NSURLConnectionDownloadDelegate
-  connectionDidFinishDownloading(\_:destinationURL:) 

Instance Method

# connectionDidFinishDownloading(\_:destinationURL:)

Sent to the delegate when the URL connection has successfully downloaded the URL asset to a destination file.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func connectionDidFinishDownloading(
    _ connection: NSURLConnection,
    destinationURL: URL
)
```

**Required**

## Parameters 

`connection`  

The URL connection object that downloaded the asset.

`destinationURL`  

A file URL specifying a destination in the file system. For iOS applications, this is a location in the application sandbox.

## Discussion

This method will be called once after a successful download. The file downloaded to `destinationURL` is guaranteed to exist there only for the duration of this method implementation; the delegate should copy or move the file to a more persistent and appropriate location.

## See Also

### Managing Downloads of URL Assets

func connection(NSURLConnection, didWriteData: Int64, totalBytesWritten: Int64, expectedTotalBytes: Int64)

Sent to the delegate to deliver progress information for a download of a URL asset to a destination file.

func connectionDidResumeDownloading(NSURLConnection, totalBytesWritten: Int64, expectedTotalBytes: Int64)

Sent to the delegate when an URL connection resumes downloading a URL asset that was earlier suspended.

