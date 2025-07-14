

- Foundation
- NSURLDownload
-  deletesFileUponFailure 

Instance Property

# deletesFileUponFailure

Returns whether the receiver deletes partially downloaded files when a download stops prematurely.

macOS 10.2+

``` source
var deletesFileUponFailure: Bool { get set }
```

## Return Value

true if partially downloaded files should be deleted when a download stops prematurely, false otherwise. The default is true.

## See Also

### Resuming partial downloads

class func canResumeDownloadDecoded(withEncodingMIMEType: String) -> Bool

Returns whether a URL download object can resume a download that was decoded with the specified MIME type.

init(resumeData: Data, delegate: (any NSURLDownloadDelegate)?, path: String)

Returns an initialized NSURLDownload object that will resume downloading the specified data to the specified file and begins the download.

Deprecated

var resumeData: Data?

Returns the resume data for a download that is not yet complete.

