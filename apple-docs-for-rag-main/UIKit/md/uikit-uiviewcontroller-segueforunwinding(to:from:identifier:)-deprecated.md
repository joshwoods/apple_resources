

- UIKit
- UIViewController
-  segueForUnwinding(to:from:identifier:) Deprecated

Instance Method

# segueForUnwinding(to:from:identifier:)

Called when an unwind segue action needs to transition between two view controllers.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func segueForUnwinding(
    to toViewController: UIViewController,
    from fromViewController: UIViewController,
    identifier: String?
) -> UIStoryboardSegue?
```

Deprecated

Use unwind(for:towards:) instead.

## Parameters 

`toViewController`  

The target view controller.

`fromViewController`  

The view controller initiating the unwind action.

`identifier`  

An identifier for the segue.

## Return Value

A segue object for managing the transitions between the two view controllers.

## Discussion

If you implement a custom container view controller that also uses segue unwinding, you must override this method. In your custom implementation, instantiate and return a segue object that performs whatever animation and other steps that are necessary to unwind the view controllers.

You do not need to override this method for view controllers that are not containers.

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

func shouldAutomaticallyForwardRotationMethods() -> Bool

Returns a Boolean value indicating whether rotation methods are forwarded to child view controllers.

Deprecated

func willAnimateRotation(to: UIInterfaceOrientation, duration: TimeInterval)

Sent to the view controller before performing a one-step user interface rotation.

Deprecated

func willRotate(to: UIInterfaceOrientation, duration: TimeInterval)

Sent to the view controller just before the user interface begins rotating.

Deprecated

