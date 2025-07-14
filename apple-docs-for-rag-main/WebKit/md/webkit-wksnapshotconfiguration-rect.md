

- WebKit
- WKSnapshotConfiguration
-  rect 

Instance Property

# rect

The portion of your web view to capture, specified as a rectangle in the view’s coordinate system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
@MainActor
var rect: CGRect { get set }
```

## Discussion

The default value of this property is CGRectNull, which captures everything in the view’s bounds rectangle. If you specify a custom rectangle, it must lie within the bounds rectangle of the WKWebView object.

## See Also

### Specifying the snapshot dimensions

var snapshotWidth: NSNumber?

The width of the captured image, in points.

