

- WebKit
- WKNavigationAction
-  targetFrame 

Instance Property

# targetFrame

The frame in which to display the new content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@NSCopying @MainActor
var targetFrame: WKFrameInfo? { get }
```

## Discussion

If the target of the navigation is a new window, this property is `nil`.

## See Also

### Inspecting navigation information

var request: URLRequest

The URL request object associated with the navigation action.

var sourceFrame: WKFrameInfo

The frame that requested the navigation.

var shouldPerformDownload: Bool

A Boolean value that indicates whether the web content provided an attribute that indicates a download.

