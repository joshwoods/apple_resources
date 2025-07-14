

- UIKit
- UILargeContentViewerInteractionDelegate
-  largeContentViewerInteraction(\_:didEndOn:at:) 

Instance Method

# largeContentViewerInteraction(\_:didEndOn:at:)

Performs an action when the large content viewer gesture ends at the location of the specified item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func largeContentViewerInteraction(
    _ interaction: UILargeContentViewerInteraction,
    didEndOn item: (any UILargeContentViewerItem)?,
    at point: CGPoint
)
```

## Parameters 

`interaction`  

The large content viewer interaction associated with the view that the user interacted with.

`item`  

The item that the user interacted with in the large content viewer.

`point`  

The point where the user’s interaction ended, in the coordinate space of the item’s view.

## Discussion

If you don’t implement this method and are using standard UIKit controls, the system performs a default action, such as sending a touchUpInside event to the control. If you’re using a custom view with its own tap gesture recognizer, implement this method to handle the interaction. For example, to perform the action that would have occurred if the user tapped on that item.

UIKit only calls this method if the gesture ends successfully, not if it fails or gets canceled.

## See Also

### Customizing large content viewer interactions

func largeContentViewerInteraction(UILargeContentViewerInteraction, itemAt: CGPoint) -> (any UILargeContentViewerItem)?

Identifies the large content viewer item for the specified interaction and location.

func viewController(for: UILargeContentViewerInteraction) -> UIViewController

Specifies which view controller should display the large content viewer.

