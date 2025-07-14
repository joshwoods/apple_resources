

- UIKit
- UIModalPresentationStyle
-  UIModalPresentationStyle.pageSheet 

Case

# UIModalPresentationStyle.pageSheet

A presentation style that partially covers the underlying content.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
case pageSheet
```

## Discussion

In a regular-width, regular-height size class, the system adds a dimming layer over the background content and centers the view controller’s content on top of this layer. The content is roughly the size of a page, where the height is greater than the width. The actual dimensions vary depending on several factors including the device’s screen size and orientation. A part of the background content always remains visible.

To provide a custom content size, use the UIModalPresentationStyle.formSheet style instead, and set the modal view controller’s preferredContentSize property.

In a compact-width, regular-height size class, the system displays the view controller as a sheet with part of the background content visible near the top of the screen.

In a compact-height size class, the behavior is the same as UIModalPresentationStyle.fullScreen.

Where the background content remains visible, the system doesn’t call the presenting view controller’s viewWillDisappear(_:) and viewDidDisappear(_:) methods.

## See Also

### Presentations

case automatic

The default presentation style chosen by the system.

case none

A presentation style that indicates no adaptations should be made.

case fullScreen

A presentation style in which the presented view covers the screen.

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

