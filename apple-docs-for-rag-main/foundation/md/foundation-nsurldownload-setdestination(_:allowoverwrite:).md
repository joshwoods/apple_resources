

- Foundation
- NSURLDownload
-  setDestination(\_:allowOverwrite:) 

Instance Method

# setDestination(\_:allowOverwrite:)

Sets the destination path of the downloaded file.

macOS 10.2+

``` source
func setDestination(
    _ path: String,
    allowOverwrite: Bool
)
```

## Parameters 

`path`  

The path for the downloaded file.

`allowOverwrite`  

true if an existing file at `path` can be replaced, false otherwise.

## Discussion

If `allowOverwrite` is false and a file already exists at `path`, a unique filename will be created for the downloaded file by appending a number to the filename. The delegate can implement the download(_:didCreateDestination:) delegate method to determine the filename used when the file is written to disk.

### Special Considerations

An `NSURLDownload` instance ignores multiple calls to this method.

## See Also

### Related Documentation

func download(NSURLDownload, decideDestinationWithSuggestedFilename: String)

The delegate receives this message when `download` has determined a suggested filename for the downloaded file.

func download(NSURLDownload, didCreateDestination: String)

Sent when the destination file is created.

### Creating and configuring a download instance

init(request: URLRequest, delegate: (any NSURLDownloadDelegate)?)

Returns an initialized URL download for a URL request and begins to download the data for the request.

Deprecated

