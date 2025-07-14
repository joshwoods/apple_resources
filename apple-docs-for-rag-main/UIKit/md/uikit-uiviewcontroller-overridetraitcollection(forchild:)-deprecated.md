

- UIKit
- UIViewController
-  overrideTraitCollection(forChild:) Deprecated

Instance Method

# overrideTraitCollection(forChild:)

Retrieves the trait collection for a child view controller.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func overrideTraitCollection(forChild childViewController: UIViewController) -> UITraitCollection?
```

## Parameters 

`childViewController`  

The view controller who’s trait collection is to be returned.

## Return Value

The trait collection for the designated view controller.

## Discussion

Use this method to retrieve the trait collection for a child view controller. You can then modify the trait collection for the designated child view controller and set it using the setOverrideTraitCollection(_:forChild:) method.

## See Also

### Deprecated methods

func setOverrideTraitCollection(UITraitCollection?, forChild: UIViewController)

Changes the traits assigned to the specified child view controller.

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

func willRotate(to: UIInterfaceOrientation, duration: TimeInterval)

Sent to the view controller just before the user interface begins rotating.

Deprecated

