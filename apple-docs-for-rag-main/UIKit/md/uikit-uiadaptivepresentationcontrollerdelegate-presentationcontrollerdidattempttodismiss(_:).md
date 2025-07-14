

- UIKit
- UIAdaptivePresentationControllerDelegate
-  presentationControllerDidAttemptToDismiss(\_:) 

Instance Method

# presentationControllerDidAttemptToDismiss(\_:)

Notifies the delegate that a user-initiated attempt to dismiss a view was prevented.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func presentationControllerDidAttemptToDismiss(_ presentationController: UIPresentationController)
```

## Parameters 

`presentationController`  

The presentation controller managing the adaptivity change.

## Discussion

UIKit supports refusing to dismiss a presentation when the `presentationController`.isModalInPresentation returns `true` or presentationControllerShouldDismiss(_:) returns `false`.

Use this method to inform the user why the presentation can’t be dismissed, for example, by presenting an instance of UIAlertController.

## See Also

### Responding to adaptive transitions

func presentationController(UIPresentationController, willPresentWithAdaptiveStyle: UIModalPresentationStyle, transitionCoordinator: (any UIViewControllerTransitionCoordinator)?)

Notifies the delegate that an adaptivity-related transition is about to occur.

func presentationControllerShouldDismiss(UIPresentationController) -> Bool

Asks the delegate for permission to dismiss the presentation.

func presentationControllerDidDismiss(UIPresentationController)

Notifies the delegate after a presentation is dismissed.

func presentationControllerWillDismiss(UIPresentationController)

Notifies the delegate before a presentation is dismissed.

