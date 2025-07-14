

- WebKit
- WKNavigationResponse
-  isForMainFrame 

Instance Property

# isForMainFrame

A Boolean value that indicates whether the response targets the web view’s main frame.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var isForMainFrame: Bool { get }
```

## Discussion

The value of this property is true if the response targets the main frame. The value is false if the response targets a different frame, such as the frame in a new window.

## See Also

### Getting Additional Response Information

var canShowMIMEType: Bool

A Boolean value that indicates whether WebKit is capable of displaying the response’s MIME type natively.

