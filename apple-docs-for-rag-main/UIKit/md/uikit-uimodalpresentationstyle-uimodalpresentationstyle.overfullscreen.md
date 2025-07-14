

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.overFullScreen 

Case

# UIModalPresentationStyle.overFullScreen

A view presentation style in which the presented view covers the screen.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case overFullScreen
```

## Discussion

The views beneath the presented content are not removed from the view hierarchy when the presentation finishes. So if the presented view controller does not fill the screen with opaque content, the underlying content shows through.

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

case overCurrentContext

A presentation style where the content is displayed over another view controller’s content.

case popover

A presentation style where the content is displayed in a popover view.

case blurOverFullScreen

A presentation style that blurs the underlying content before displaying new content in a full-screen presentation.

