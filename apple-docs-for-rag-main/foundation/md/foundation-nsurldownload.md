

- Foundation
-  NSURLDownload 

Class

# NSURLDownload

An object that downloads a resource asynchronously and saves the data to a file.

macOS 10.2+

``` source
class NSURLDownload
```

## Overview

Important

This API is considered legacy. Use URLSession instead.

The interface for NSURLDownload provides methods to initialize a download, set the destination path and cancel loading the request.

The delegate object assigned to each instance of this class should implement the methods defined by the NSURLDownloadDelegate protocol. These methods provide the delegate with the current status of in-progress asynchronous downloads and allow the delegate to customize the URL loading process. These delegate methods are called on the thread that started the asynchronous load operation for the associated NSURLDownload object.

## Topics

### Creating and configuring a download instance

init(request: URLRequest, delegate: (any NSURLDownloadDelegate)?)

Returns an initialized URL download for a URL request and begins to download the data for the request.

Deprecated

func setDestination(String, allowOverwrite: Bool)

Sets the destination path of the downloaded file.

### Resuming partial downloads

class func canResumeDownloadDecoded(withEncodingMIMEType: String) -> Bool

Returns whether a URL download object can resume a download that was decoded with the specified MIME type.

init(resumeData: Data, delegate: (any NSURLDownloadDelegate)?, path: String)

Returns an initialized NSURLDownload object that will resume downloading the specified data to the specified file and begins the download.

Deprecated

var resumeData: Data?

Returns the resume data for a download that is not yet complete.

var deletesFileUponFailure: Bool

Returns whether the receiver deletes partially downloaded files when a download stops prematurely.

### Canceling a download

func cancel()

Cancels the receiver’s download and deletes the downloaded file.

### Getting download properties

var request: URLRequest

Returns the request that initiated the receiver’s download.

var deletesFileUponFailure: Bool

Returns whether the receiver deletes partially downloaded files when a download stops prematurely.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### URL Download

protocol NSURLDownloadDelegate

A protocol that URL download delegates implement to interact with a URL download request.

