

- WebKit
- WKNavigationAction
-  shouldPerformDownload 

Instance Property

# shouldPerformDownload

A Boolean value that indicates whether the web content provided an attribute that indicates a download.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+visionOS 1.0+

``` source
@MainActor
var shouldPerformDownload: Bool { get }
```

## See Also

### Inspecting navigation information

var request: URLRequest

The URL request object associated with the navigation action.

var sourceFrame: WKFrameInfo

The frame that requested the navigation.

var targetFrame: WKFrameInfo?

The frame in which to display the new content.

