

- UIKit
- UIViewController
-  forUnwindSegueAction(\_:from:withSender:) Deprecated

Instance Method

# forUnwindSegueAction(\_:from:withSender:)

Called when an unwind segue action wants to search a container’s children for a view controller to handle the unwind action.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func forUnwindSegueAction(
    _ action: Selector,
    from fromViewController: UIViewController,
    withSender sender: Any?
) -> UIViewController?
```

Deprecated

Override the allowedChildrenForUnwinding(from:) method instead.

## Parameters 

`action`  

The action that triggered the unwind action.

`fromViewController`  

The view controller that is the source of the unwinding action.

`sender`  

The object that initiated the action.

## Return Value

The view controller that wants to handle the unwind action.

## Discussion

A custom container view controller should override this method and use it to search its children for a view controller to handle the unwind action. It does this by invoking the canPerformUnwindSegueAction(_:from:withSender:) method on each child. If a view controller wants to handle the action, your method should return it. If none of the container’s children want to handle the unwind action, invoke the super’s implementation and return the result of that method.

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

