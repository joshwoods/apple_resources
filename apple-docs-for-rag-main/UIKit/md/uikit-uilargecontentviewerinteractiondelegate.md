

- UIKit
-  UILargeContentViewerInteractionDelegate 

Protocol

# UILargeContentViewerInteractionDelegate

An object that customizes the behavior of the large content viewer interactions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UILargeContentViewerInteractionDelegate : NSObjectProtocol
```

## Topics

### Customizing large content viewer interactions

func largeContentViewerInteraction(UILargeContentViewerInteraction, didEndOn: (any UILargeContentViewerItem)?, at: CGPoint)

Performs an action when the large content viewer gesture ends at the location of the specified item.

func largeContentViewerInteraction(UILargeContentViewerInteraction, itemAt: CGPoint) -> (any UILargeContentViewerItem)?

Identifies the large content viewer item for the specified interaction and location.

func viewController(for: UILargeContentViewerInteraction) -> UIViewController

Specifies which view controller should display the large content viewer.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Content viewer

class UILargeContentViewerInteraction

An interaction that enables a gesture to present the large content viewer for cases when supporting the largest dynamic type sizes isn’t appropriate.

protocol UILargeContentViewerItem

Methods that provide details about how to display your custom content in the large content viewer.

