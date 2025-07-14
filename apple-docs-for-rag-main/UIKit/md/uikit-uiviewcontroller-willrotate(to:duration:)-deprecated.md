

- UIKit
- UIViewController
-  willRotate(to:duration:) Deprecated

Instance Method

# willRotate(to:duration:)

Sent to the view controller just before the user interface begins rotating.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func willRotate(
    to toInterfaceOrientation: UIInterfaceOrientation,
    duration: TimeInterval
)
```

Deprecated

Use viewWillTransition(to:with:) to make interface-based adjustments.

## Parameters 

`toInterfaceOrientation`  

The new orientation for the user interface. The possible values are described in UIInterfaceOrientation.

`duration`  

The duration of the pending rotation, measured in seconds.

## Discussion

Subclasses may override this method to perform additional actions immediately prior to the rotation. For example, you might use this method to disable view interactions, stop media playback, or temporarily turn off expensive drawing or live updates. You might also use it to swap the current view for one that reflects the new interface orientation. When this method is called, the interfaceOrientation property still contains the view’s original orientation. Your implementation of this method must call `super` at some point during its execution.

This method is called regardless of whether your code performs one-step or two-step rotations.

## See Also

### Deprecated methods

func setOverrideTraitCollection(UITraitCollection?, forChild: UIViewController)

Changes the traits assigned to the specified child view controller.

Deprecated

func overrideTraitCollection(forChild: UIViewController) -> UITraitCollection?

Retrieves the trait collection for a child view controller.

Deprecated

class func attemptRotationToDeviceOrientation()

Attempts to rotate all windows to the orientation of the device.

Deprecated

func registerForPreviewing(with: any UIViewControllerPreviewingDelegate, sourceView: UIView) -> any UIViewControllerPreviewing

Registers a view controller to participate with 3D Touch preview (peek) and commit (pop).

Deprecated

func unregisterForPreviewing(withContext: any UIViewControllerPreviewing)

Unregisters a previously registered view controller identified by its context object.

Deprecated

func canPerformUnwindSegueAction(Selector, from: UIViewController, withSender: Any) -> Bool

Called on a view controller to determine whether it wants to respond to an unwind action.

Deprecated

func didRotate(from: UIInterfaceOrientation)

Sent to the view controller after the user interface rotates.

Deprecated

func dismissMoviePlayerViewControllerAnimated()

Dismisses a movie player view controller using the standard movie player transition.

Deprecated

func forUnwindSegueAction(Selector, from: UIViewController, withSender: Any?) -> UIViewController?

Called when an unwind segue action wants to search a container’s children for a view controller to handle the unwind action.

Deprecated

func presentMoviePlayerViewControllerAnimated(MPMoviePlayerViewController!)

Presents the movie player view controller using the standard movie player transition.

Deprecated

func rotatingFooterView() -> UIView?

Returns the footer view to transition during an interface orientation change.

Deprecated

func rotatingHeaderView() -> UIView?

Returns the header view to transition during an interface orientation change.

Deprecated

func segueForUnwinding(to: UIViewController, from: UIViewController, identifier: String?) -> UIStoryboardSegue?

Called when an unwind segue action needs to transition between two view controllers.

Deprecated

func shouldAutomaticallyForwardRotationMethods() -> Bool

Returns a Boolean value indicating whether rotation methods are forwarded to child view controllers.

Deprecated

func willAnimateRotation(to: UIInterfaceOrientation, duration: TimeInterval)

Sent to the view controller before performing a one-step user interface rotation.

Deprecated

