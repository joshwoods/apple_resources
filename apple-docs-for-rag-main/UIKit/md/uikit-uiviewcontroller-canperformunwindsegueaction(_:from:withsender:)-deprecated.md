

- UIKit
- UIViewController
-  canPerformUnwindSegueAction(\_:from:withSender:) Deprecated

Instance Method

# canPerformUnwindSegueAction(\_:from:withSender:)

Called on a view controller to determine whether it wants to respond to an unwind action.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
func canPerformUnwindSegueAction(
    _ action: Selector,
    from fromViewController: UIViewController,
    withSender sender: Any
) -> Bool
```

## Parameters 

`action`  

The unwind action to invoke on your view controller.

`fromViewController`  

The view controller that initiated the unwind action.

`sender`  

The object that triggered the action.

## Return Value

true if the view controller wants to handle the unwind action, otherwise false.

## Discussion

When an unwind segue is triggered, UIKit uses this method and the allowedChildrenForUnwinding(from:) method to locate a suitable view controller to handle the unwind segue.

The default implementation of this method returns true when the current view controller implements the `action` method and is not the same view controller as the one in the `fromViewController` parameter. You can override this method as needed to change the default behavior. For example, you might return false if the current view controller does not make a suitable return target when unwinding from the specified view controller.

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

func willRotate(to: UIInterfaceOrientation, duration: TimeInterval)

Sent to the view controller just before the user interface begins rotating.

Deprecated

