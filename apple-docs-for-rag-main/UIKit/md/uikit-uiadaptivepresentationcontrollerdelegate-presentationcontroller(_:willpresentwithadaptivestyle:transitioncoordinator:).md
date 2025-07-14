

- UIKit
- UIAdaptivePresentationControllerDelegate
-  presentationController(\_:willPresentWithAdaptiveStyle:transitionCoordinator:) 

Instance Method

# presentationController(\_:willPresentWithAdaptiveStyle:transitionCoordinator:)

Notifies the delegate that an adaptivity-related transition is about to occur.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func presentationController(
    _ presentationController: UIPresentationController,
    willPresentWithAdaptiveStyle style: UIModalPresentationStyle,
    transitionCoordinator: (any UIViewControllerTransitionCoordinator)?
)
```

## Parameters 

`presentationController`  

The presentation controller that is managing the adaptivity change.

`style`  

The new presentation style. If the presentation style is not changing, this parameter is set to UIModalPresentationStyle.none.

`transitionCoordinator`  

The transition coordinator that is managing the transition.

## Discussion

When a size class change occurs, UIKit calls this method to let you know how the presentation controller will adapt. Use this method to make any additional changes. For example, you might use the transition coordinator object to create additional animations for the transition.

## See Also

### Responding to adaptive transitions

func presentationControllerDidAttemptToDismiss(UIPresentationController)

Notifies the delegate that a user-initiated attempt to dismiss a view was prevented.

func presentationControllerShouldDismiss(UIPresentationController) -> Bool

Asks the delegate for permission to dismiss the presentation.

func presentationControllerDidDismiss(UIPresentationController)

Notifies the delegate after a presentation is dismissed.

func presentationControllerWillDismiss(UIPresentationController)

Notifies the delegate before a presentation is dismissed.

