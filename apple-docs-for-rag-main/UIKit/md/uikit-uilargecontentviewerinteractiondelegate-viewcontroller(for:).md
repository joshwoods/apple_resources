

- UIKit
- UILargeContentViewerInteractionDelegate
-  viewController(for:) 

Instance Method

# viewController(for:)

Specifies which view controller should display the large content viewer.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
optional func viewController(for interaction: UILargeContentViewerInteraction) -> UIViewController
```

## Parameters 

`interaction`  

The large content viewer that the system is displaying.

## Return Value

A view controller that the system uses to present the large content viewer in.

## Discussion

By default, UIKit uses a view controller that contains the view you added the interaction to. If this default choice doesn’t work for your app, implement this method to specify a different view controller.

## See Also

### Customizing large content viewer interactions

func largeContentViewerInteraction(UILargeContentViewerInteraction, didEndOn: (any UILargeContentViewerItem)?, at: CGPoint)

Performs an action when the large content viewer gesture ends at the location of the specified item.

func largeContentViewerInteraction(UILargeContentViewerInteraction, itemAt: CGPoint) -> (any UILargeContentViewerItem)?

Identifies the large content viewer item for the specified interaction and location.

