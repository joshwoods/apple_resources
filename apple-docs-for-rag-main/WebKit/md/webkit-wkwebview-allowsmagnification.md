

- WebKit
- WKWebView
-  allowsMagnification 

Instance Property

# allowsMagnification

A Boolean value that indicates whether magnify gestures change the web view’s magnification.

macOS 10.10+

``` source
@MainActor
var allowsMagnification: Bool { get set }
```

## Discussion

The default value is false. You can set the `magnification` property even if `allowsMagnification` is set to false.

## See Also

### Scaling content

var pageZoom: CGFloat

The scale factor by which the web view scales content relative to its bounds.

var magnification: CGFloat

The factor by which the page content is currently scaled.

func setMagnification(CGFloat, centeredAt: CGPoint)

Scales the page content and centers the result on the specified point.

