

- UIKit
- UIAdaptivePresentationControllerDelegate
-  presentationControllerShouldDismiss(\_:) 

Instance Method

# presentationControllerShouldDismiss(\_:)

Asks the delegate for permission to dismiss the presentation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func presentationControllerShouldDismiss(_ presentationController: UIPresentationController) -> Bool
```

## Parameters 

`presentationController`  

The presentation controller that manages the adaptivity change.

## Return Value

true to allow the system to dismiss the presentation, false to refuse the dismissal.

## Discussion

The system may call this method at any time. This method isn’t guaranteed to be followed by a call to presentationControllerWillDismiss(_:) or presentationControllerDidDismiss(_:). Make sure that your implementation of this method returns quickly.

## See Also

### Related Documentation

Disabling the pull-down gesture for a sheet

Ensure a positive user experience when presenting a view controller as a sheet.

### Responding to adaptive transitions

func presentationController(UIPresentationController, willPresentWithAdaptiveStyle: UIModalPresentationStyle, transitionCoordinator: (any UIViewControllerTransitionCoordinator)?)

Notifies the delegate that an adaptivity-related transition is about to occur.

func presentationControllerDidAttemptToDismiss(UIPresentationController)

Notifies the delegate that a user-initiated attempt to dismiss a view was prevented.

func presentationControllerDidDismiss(UIPresentationController)

Notifies the delegate after a presentation is dismissed.

func presentationControllerWillDismiss(UIPresentationController)

Notifies the delegate before a presentation is dismissed.

