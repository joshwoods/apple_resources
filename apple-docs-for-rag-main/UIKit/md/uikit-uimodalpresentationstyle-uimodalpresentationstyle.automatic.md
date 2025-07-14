

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.automatic 

Case

# UIModalPresentationStyle.automatic

The default presentation style chosen by the system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
case automatic
```

## Discussion

For most view controllers, UIKit maps this style to:

- UIModalPresentationStyle.formSheet in iOS 18 and later

- UIModalPresentationStyle.pageSheet in versions of iOS earlier than iOS 18

Some system view controllers may map it to a different style.

## See Also

### Presentations

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

case overCurrentContext

A presentation style where the content is displayed over another view controller’s content.

case popover

A presentation style where the content is displayed in a popover view.

case blurOverFullScreen

A presentation style that blurs the underlying content before displaying new content in a full-screen presentation.

