

- WebKit
- WKWebView
-  pageZoom 

Instance Property

# pageZoom

The scale factor by which the web view scales content relative to its bounds.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
@MainActor
var pageZoom: CGFloat { get set }
```

## Discussion

The default value of this property is `1.0`, which displays the content without any scaling. Changing the value of this property is equivalent to setting the CSS `zoom` property on all page content.

## See Also

### Scaling content

var allowsMagnification: Bool

A Boolean value that indicates whether magnify gestures change the web view’s magnification.

var magnification: CGFloat

The factor by which the page content is currently scaled.

func setMagnification(CGFloat, centeredAt: CGPoint)

Scales the page content and centers the result on the specified point.

