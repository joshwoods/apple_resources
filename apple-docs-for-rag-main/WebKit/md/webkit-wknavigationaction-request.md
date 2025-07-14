

- WebKit
- WKNavigationAction
-  request 

Instance Property

# request

The URL request object associated with the navigation action.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var request: URLRequest { get }
```

## See Also

### Inspecting navigation information

var sourceFrame: WKFrameInfo

The frame that requested the navigation.

var targetFrame: WKFrameInfo?

The frame in which to display the new content.

var shouldPerformDownload: Bool

A Boolean value that indicates whether the web content provided an attribute that indicates a download.

