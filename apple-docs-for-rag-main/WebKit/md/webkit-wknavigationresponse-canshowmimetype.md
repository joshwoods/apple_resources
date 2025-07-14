

- WebKit
- WKNavigationResponse
-  canShowMIMEType 

Instance Property

# canShowMIMEType

A Boolean value that indicates whether WebKit is capable of displaying the response’s MIME type natively.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
@MainActor
var canShowMIMEType: Bool { get }
```

## Discussion

The value of this property is true if WebKit is able to display the MIME type.

## See Also

### Getting Additional Response Information

var isForMainFrame: Bool

A Boolean value that indicates whether the response targets the web view’s main frame.

