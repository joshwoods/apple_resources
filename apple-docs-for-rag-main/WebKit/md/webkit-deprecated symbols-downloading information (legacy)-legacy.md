

- WebKit
- Deprecated Symbols
-  Downloading Information (Legacy) 

API Collection

# Downloading Information (Legacy)

## Topics

### Downloading Information (Legacy)

class WebDownload

`WebDownload` objects initiate download client requests on behalf of a delegate. A download request involves loading the data, decoding it (if necessary), and saving it to a file. Instances of this class behave similar to `NSURLDownload` except delegates of `WebDownload` may implement an additional delegate method. The method allows the delegate to specify the window to be used for authentication sheets. If the delegate does not implement this method, the `WebDownload` object will prompt the user for authentication using the standard WebKit authentication panel, as either a sheet or window. There are no additional methods defined in this class. See WebDownloadDelegate for the delegate method.

Deprecated

protocol WebDownloadDelegate

The `WebDownloadDelegate` protocol declares one additional method for delegates of WebDownload.

Deprecated

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

URL Loading System

Interact with URLs and communicate with servers using standard Internet protocols.

### WebKit Legacy APIs

Document Object Models API (Legacy)

Setting Up a Web View (Legacy)

Accessing Previous Webpages (Legacy)

Archiving Webpages (Legacy)

Loading Resources (Legacy)

Working with Frames (legacy)

Opening a File (Legacy)

Setting Policies (Legacy)

Implementing Plugins (Legacy)

Incorporating Scripts (Legacy)

Working With Document Web Views (Legacy)

