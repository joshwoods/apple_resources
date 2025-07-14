

- WebKit
- WKWebView
-  setMagnification(\_:centeredAt:) 

Instance Method

# setMagnification(\_:centeredAt:)

Scales the page content and centers the result on the specified point.

macOS 10.10+

``` source
@MainActor
func setMagnification(
    _ magnification: CGFloat,
    centeredAt point: CGPoint
)
```

## Parameters 

`magnification`  

The factor by which to scale the content.

`point`  

The point (in the web view’s bounds) at which to center magnification.

## See Also

### Scaling content

var pageZoom: CGFloat

The scale factor by which the web view scales content relative to its bounds.

var allowsMagnification: Bool

A Boolean value that indicates whether magnify gestures change the web view’s magnification.

var magnification: CGFloat

The factor by which the page content is currently scaled.

