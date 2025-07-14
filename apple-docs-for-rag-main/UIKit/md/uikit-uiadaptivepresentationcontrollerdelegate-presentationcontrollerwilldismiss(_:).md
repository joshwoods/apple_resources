

- UIKit
- UIAdaptivePresentationControllerDelegate
-  presentationControllerWillDismiss(\_:) 

Instance Method

# presentationControllerWillDismiss(\_:)

Notifies the delegate before a presentation is dismissed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func presentationControllerWillDismiss(_ presentationController: UIPresentationController)
```

## Parameters 

`presentationController`  

The presentation controller managing the trait changes from your app.

## Discussion

You can use this method to set up animations or interaction notifications with the presentationController’s transitionCoordinator.

This method is not called if the presentation is dismissed programmatically.

## See Also

### Responding to adaptive transitions

func presentationController(UIPresentationController, willPresentWithAdaptiveStyle: UIModalPresentationStyle, transitionCoordinator: (any UIViewControllerTransitionCoordinator)?)

Notifies the delegate that an adaptivity-related transition is about to occur.

func presentationControllerDidAttemptToDismiss(UIPresentationController)

Notifies the delegate that a user-initiated attempt to dismiss a view was prevented.

func presentationControllerShouldDismiss(UIPresentationController) -> Bool

Asks the delegate for permission to dismiss the presentation.

func presentationControllerDidDismiss(UIPresentationController)

Notifies the delegate after a presentation is dismissed.

