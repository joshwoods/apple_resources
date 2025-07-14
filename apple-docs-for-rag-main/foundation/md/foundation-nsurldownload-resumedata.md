

- Foundation
- NSURLDownload
-  resumeData 

Instance Property

# resumeData

Returns the resume data for a download that is not yet complete.

macOS 10.2+

``` source
var resumeData: Data? { get }
```

## Return Value

The resume data for a download that is not yet complete. This data represents the necessary state information that an `NSURLDownload` object needs to resume a download. The resume data can later be used when initializing a download with init(resumeData:delegate:path:). Returns `nil` if the download is not able to be resumed.

## Discussion

Resume data is returned only if both the protocol and the server support resuming. For details on how to resume a connection, see the documentation for init(resumeData:delegate:path:).

## See Also

### Resuming partial downloads

class func canResumeDownloadDecoded(withEncodingMIMEType: String) -> Bool

Returns whether a URL download object can resume a download that was decoded with the specified MIME type.

init(resumeData: Data, delegate: (any NSURLDownloadDelegate)?, path: String)

Returns an initialized NSURLDownload object that will resume downloading the specified data to the specified file and begins the download.

Deprecated

var deletesFileUponFailure: Bool

Returns whether the receiver deletes partially downloaded files when a download stops prematurely.

