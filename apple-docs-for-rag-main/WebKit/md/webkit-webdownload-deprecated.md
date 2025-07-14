

- WebKit
-  WebDownload Deprecated

Class

# WebDownload

`WebDownload` objects initiate download client requests on behalf of a delegate. A download request involves loading the data, decoding it (if necessary), and saving it to a file. Instances of this class behave similar to `NSURLDownload` except delegates of `WebDownload` may implement an additional delegate method. The method allows the delegate to specify the window to be used for authentication sheets. If the delegate does not implement this method, the `WebDownload` object will prompt the user for authentication using the standard WebKit authentication panel, as either a sheet or window. There are no additional methods defined in this class. See WebDownloadDelegate for the delegate method.

macOS 10.4–10.14Deprecated

``` source
class WebDownload
```

## Relationships

### Inherits From

- NSURLDownload

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Downloading Information (Legacy)

protocol WebDownloadDelegate

The `WebDownloadDelegate` protocol declares one additional method for delegates of WebDownload.

Deprecated

