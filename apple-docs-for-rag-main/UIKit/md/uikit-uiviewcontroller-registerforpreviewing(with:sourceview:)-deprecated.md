

- UIKit
- UIViewController
-  registerForPreviewing(with:sourceView:) Deprecated

Instance Method

# registerForPreviewing(with:sourceView:)

Registers a view controller to participate with 3D Touch preview (peek) and commit (pop).

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
func registerForPreviewing(
    with delegate: any UIViewControllerPreviewingDelegate,
    sourceView: UIView
) -> any UIViewControllerPreviewing
```

Deprecated

Use UIContextMenuInteraction instead.

## Parameters 

`delegate`  

The delegate object mediates the presentation of views from the preview (peek) view controller and the commit (pop) view controller. In practice, these two are typically the same view controller. The delegate performs this mediation through your implementation of the methods of the UIViewControllerPreviewingDelegate protocol.

`sourceView`  

The view, in the view hierarchy of the receiver of this method call, that invokes a preview when pressed by the user.

When lightly pressed, the source view remains visually sharp while surrounding content blurs. When pressed more deeply, the system calls the previewingContext(_:viewControllerForLocation:) method in your `delegate` object, which presents the preview (peek) view from another view controller.

## Return Value

A context object for managing the preview. This object conforms to the UIViewControllerPreviewing protocol.

## Discussion

A preview, or *peek* in end-user terminology, provides additional content related to the view the user pressed (that is, related to the `sourceView` view).

Calling this method does three things:

- Registers the previewing view controller (the one that receives this method call) to participate with 3D Touch preview and commit

- Designates the source view, from the receiver’s view hierarchy, as the view to respond to a forceful touch

- Designates a delegate object for mediating the presentation of the preview (peek) and commit (pop) views as a user requests them in turn by pressing more deeply

You can designate more than one source view for a single registered view controller, but you cannot designate a single view as a source view more than once.

The lifetime of this method’s returned context object is managed by the system. If you need to explicitly unregister a view controller, pass its context object to the unregisterForPreviewing(withContext:) method. If you do not unregister a view controller, the system automatically unregisters it when the view controller is deallocated.

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

