

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.overCurrentContext 

Case

# UIModalPresentationStyle.overCurrentContext

A presentation style where the content is displayed over another view controller’s content.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case overCurrentContext
```

## Discussion

Using this presentation style, the current view controller’s content is displayed over the view controller whose definesPresentationContext property is true. UIKit may walk up the view controller hierarchy to find a view controller that wants to define the presentation context. The views beneath the presented content are not removed from the view hierarchy when the presentation finishes. So if the presented view controller does not fill the screen with opaque content, the underlying content shows through.

When presenting a view controller in a popover, this presentation style is supported only if the transition style is UIModalTransitionStyle.coverVertical. Attempting to use a different transition style triggers an exception. However, you may use other transition styles (except the partial curl transition) if the parent view controller is not in a popover.

## See Also

### Presentations

case automatic

The default presentation style chosen by the system.

case none

A presentation style that indicates no adaptations should be made.

case fullScreen

A presentation style in which the presented view covers the screen.

case pageSheet

A presentation style that partially covers the underlying content.

case formSheet

A presentation style that displays the content centered in the screen.

case currentContext

A presentation style where the content is displayed over another view controller’s content.

case custom

A custom view presentation style that is managed by a custom presentation controller and one or more custom animator objects.

case overFullScreen

A view presentation style in which the presented view covers the screen.

case popover

A presentation style where the content is displayed in a popover view.

case blurOverFullScreen

A presentation style that blurs the underlying content before displaying new content in a full-screen presentation.

