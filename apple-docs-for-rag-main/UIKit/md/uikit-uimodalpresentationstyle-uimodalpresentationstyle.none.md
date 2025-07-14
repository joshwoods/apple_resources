

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.none 

Case

# UIModalPresentationStyle.none

A presentation style that indicates no adaptations should be made.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case none
```

## Discussion

Do not use this style to present a view controller. Instead, return it from the adaptivePresentationStyle(for:) method of an adaptive delegate when you do not want a presentation controller to adapt the style of an already presented view controller.

## See Also

### Presentations

case automatic

The default presentation style chosen by the system.

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

case overCurrentContext

A presentation style where the content is displayed over another view controller’s content.

case popover

A presentation style where the content is displayed in a popover view.

case blurOverFullScreen

A presentation style that blurs the underlying content before displaying new content in a full-screen presentation.

