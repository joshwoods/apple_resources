

- UIKit
- UIViewController
-  prepare(for:sender:) 

Instance Method

# prepare(for:sender:)

Notifies the view controller that a segue is about to be performed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func prepare(
    for segue: UIStoryboardSegue,
    sender: Any?
)
```

## Parameters 

`segue`  

The segue object containing information about the view controllers involved in the segue.

`sender`  

The object that initiated the segue. You might use this parameter to perform different actions based on which control (or other object) initiated the segue.

## Mentioned in 

Customizing the behavior of segue-based presentations

## Discussion

The default implementation of this method does nothing. Subclasses override this method and use it to configure the new view controller prior to it being displayed. The segue object contains information about the transition, including references to both view controllers that are involved.

Because segues can be triggered from multiple sources, you can use the information in the `segue` and `sender` parameters to disambiguate between different logical paths in your app. For example, if the segue originated from a table view, the sender parameter would identify the table view cell that the user tapped. You could then use that information to set the data on the destination view controller.

## See Also

### Performing segues

func shouldPerformSegue(withIdentifier: String, sender: Any?) -> Bool

Determines whether the segue with the specified identifier should be performed.

func performSegue(withIdentifier: String, sender: Any?)

Initiates the segue with the specified identifier from the current view controller’s storyboard file.

func allowedChildrenForUnwinding(from: UIStoryboardUnwindSegueSource) -> [UIViewController]

Returns an array of child view controllers to search for an unwind segue destination.

func childContaining(UIStoryboardUnwindSegueSource) -> UIViewController?

Returns the child view controller that contains the source of the unwind segue.

func canPerformUnwindSegueAction(Selector, from: UIViewController, sender: Any?) -> Bool

Called on a view controller to determine whether it responds to an unwind action.

func unwind(for: UIStoryboardSegue, towards: UIViewController)

Called when an unwind segue transitions to a new view controller.

