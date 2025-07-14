

- UIKit
- UILargeContentViewerInteractionDelegate
-  largeContentViewerInteraction(\_:itemAt:) 

Instance Method

# largeContentViewerInteraction(\_:itemAt:)

Identifies the large content viewer item for the specified interaction and location.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func largeContentViewerInteraction(
    _ interaction: UILargeContentViewerInteraction,
    itemAt point: CGPoint
) -> (any UILargeContentViewerItem)?
```

## Parameters 

`interaction`  

The large content viewer interaction that needs an item.

`point`  

The point where the user’s interaction is taking place, in the coordinate space of the view that contains the interaction.

## Discussion

By default, UIKit finds the item for the interaction by calling point(inside:with:) recursively on your view hierarchy. If you’re not using views, implement this method to identify the item for an interaction at a given point.

## See Also

### Customizing large content viewer interactions

func largeContentViewerInteraction(UILargeContentViewerInteraction, didEndOn: (any UILargeContentViewerItem)?, at: CGPoint)

Performs an action when the large content viewer gesture ends at the location of the specified item.

func viewController(for: UILargeContentViewerInteraction) -> UIViewController

Specifies which view controller should display the large content viewer.

