

- UIKit
- UIViewController
-  willAnimateRotation(to:duration:) Deprecated

Instance Method

# willAnimateRotation(to:duration:)

Sent to the view controller before performing a one-step user interface rotation.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
func willAnimateRotation(
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

This method is called from within the animation block used to rotate the view. You can override this method and use it to configure additional animations that should occur during the view rotation. For example, you could use it to adjust the zoom level of your content, change the scroller position, or modify other animatable properties of your view.

Note

The animations used to slide the header and footer views in and out of position are performed in separate animation blocks.

By the time this method is called, the interfaceOrientation property is already set to the new orientation, and the bounds of the view have been changed. Thus, you can perform any additional layout required by your views in this method.

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

func willRotate(to: UIInterfaceOrientation, duration: TimeInterval)

Sent to the view controller just before the user interface begins rotating.

Deprecated

