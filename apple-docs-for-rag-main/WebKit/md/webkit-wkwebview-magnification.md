

- WebKit
- WKWebView
-  magnification 

Instance Property

# magnification

The factor by which the page content is currently scaled.

macOS 10.10+

``` source
@MainActor
var magnification: CGFloat { get set }
```

## Discussion

The default value is `1.0`.

## See Also

### Scaling content

var pageZoom: CGFloat

The scale factor by which the web view scales content relative to its bounds.

var allowsMagnification: Bool

A Boolean value that indicates whether magnify gestures change the web view’s magnification.

func setMagnification(CGFloat, centeredAt: CGPoint)

Scales the page content and centers the result on the specified point.

