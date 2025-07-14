

- WebKit
- WKPDFConfiguration
-  rect 

Instance Property

# rect

The portion of your web view to capture, specified as a rectangle in the view’s coordinate system.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOS

``` source
@MainActor @preconcurrency
var rect: CGRect? { get set }
```

## Discussion

The default value of this property is CGRectNull, which captures everything in the view’s bounds rectangle. If you specify a custom rectangle, it must lie within the bounds rectangle of the WKWebView object.

