

- WebKit
- WKNavigationAction
-  sourceFrame 

Instance Property

# sourceFrame

The frame that requested the navigation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@NSCopying @MainActor
var sourceFrame: WKFrameInfo { get }
```

## See Also

### Inspecting navigation information

var request: URLRequest

The URL request object associated with the navigation action.

var targetFrame: WKFrameInfo?

The frame in which to display the new content.

var shouldPerformDownload: Bool

A Boolean value that indicates whether the web content provided an attribute that indicates a download.

