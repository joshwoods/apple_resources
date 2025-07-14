

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.popover 

Case

# UIModalPresentationStyle.popover

A presentation style where the content is displayed in a popover view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
case popover
```

## Discussion

In a horizontally regular environment, this style displays the view controller in a popover view. The background content is dimmed and taps outside the popover cause the popover to be dismissed. If you do not want taps to dismiss the popover, you can assign one or more views to the passthroughViews property of the associated UIPopoverPresentationController object, which you can get from the popoverPresentationController property.

In iOS 13 and later, for horizontally or vertically compact environments, this option behaves the same as UIModalPresentationStyle.formSheet.

In iOS 12 and earlier:

- For horizontally compact environments, this option behaves the same as UIModalPresentationStyle.fullScreen.

- For horizontally regular and vertically compact environments, this option behaves the same as UIModalPresentationStyle.formSheet.

For more information about horizontal and vertical size classes, see UIUserInterfaceSizeClass.

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

case overCurrentContext

A presentation style where the content is displayed over another view controller’s content.

case blurOverFullScreen

A presentation style that blurs the underlying content before displaying new content in a full-screen presentation.

