

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.custom 

Case

# UIModalPresentationStyle.custom

A custom view presentation style that is managed by a custom presentation controller and one or more custom animator objects.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
case custom
```

## Discussion

All of these objects are provided by the presented view controller’s transitioning delegate, which is an object that conforms to the UIViewControllerTransitioningDelegate protocol. Before presenting a view controller using this style, set the view controller’s transitioningDelegate property to your custom transitioning delegate.

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

case overFullScreen

A view presentation style in which the presented view covers the screen.

case overCurrentContext

A presentation style where the content is displayed over another view controller’s content.

case popover

A presentation style where the content is displayed in a popover view.

case blurOverFullScreen

A presentation style that blurs the underlying content before displaying new content in a full-screen presentation.

