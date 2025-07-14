

- Foundation
- NSURLDownload
-  canResumeDownloadDecoded(withEncodingMIMEType:) 

Type Method

# canResumeDownloadDecoded(withEncodingMIMEType:)

Returns whether a URL download object can resume a download that was decoded with the specified MIME type.

macOS 10.2+

``` source
class func canResumeDownloadDecoded(withEncodingMIMEType MIMEType: String) -> Bool
```

## Parameters 

`MIMEType`  

The MIME type the caller wants to know about.

## Return Value

true if the URL download object can resume a download that was decoded with the specified MIME type, false otherwise.

## Discussion

The MIME type of a file, in conjunction with the value returned by the download(_:shouldDecodeSourceDataOfMIMEType:) delegate method, determines whether the `NSURLDownload` class should decode or decompress the incoming data as it is received.

Some compression techniques, such as the `DEFLATE` algorithm (`gzip`) use symbol dictionaries that vary during the compression process, making it impractical to decompress only a portion of the data starting in the middle. For this reason, this method returns false unless both of the following conditions are met:

- The MIME type is of a type that the `NSURLDownload` class knows how to decompress or decode.

- The decoding can be safely resumed.

In practice, this method returns true for MacBinary and BinHex, otherwise false.

If your app needs to be able to resume file downloads in `gzip` format, your download(_:shouldDecodeSourceDataOfMIMEType:) method must return false, and you must decode the resulting file yourself after you finish downloading it in its entirety.

## See Also

### Resuming partial downloads

init(resumeData: Data, delegate: (any NSURLDownloadDelegate)?, path: String)

Returns an initialized NSURLDownload object that will resume downloading the specified data to the specified file and begins the download.

Deprecated

var resumeData: Data?

Returns the resume data for a download that is not yet complete.

var deletesFileUponFailure: Bool

Returns whether the receiver deletes partially downloaded files when a download stops prematurely.

