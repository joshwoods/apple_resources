

- UIKit
- UIViewController
-  unwind(for:towards:) 

Instance Method

# unwind(for:towards:)

Called when an unwind segue transitions to a new view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0–1.0Deprecated

``` source
@MainActor
func unwind(
    for unwindSegue: UIStoryboardSegue,
    towards subsequentVC: UIViewController
)
```

## Parameters 

`unwindSegue`  

The unwind segue being performed.

`subsequentVC`  

The view controller closest to the current controller that represents the transition direction. Container view controllers should configure themselves so that this view controller is displayed.

## Discussion

During the execution of an unwind segue, UIKit calls this method on any view controllers in the unwind path to give them an opportunity to reconfigure themselves. Container view controllers must implement this method and use to display the view controller in the `subsequentVC` parameter. For example, a tab bar controller selects the tab containing the specified view controller. Noncontainer view controllers should not override this method.

## See Also

### Performing segues

func shouldPerformSegue(withIdentifier: String, sender: Any?) -> Bool

Determines whether the segue with the specified identifier should be performed.

func prepare(for: UIStoryboardSegue, sender: Any?)

Notifies the view controller that a segue is about to be performed.

func performSegue(withIdentifier: String, sender: Any?)

Initiates the segue with the specified identifier from the current view controller’s storyboard file.

func allowedChildrenForUnwinding(from: UIStoryboardUnwindSegueSource) -> [UIViewController]

Returns an array of child view controllers to search for an unwind segue destination.

func childContaining(UIStoryboardUnwindSegueSource) -> UIViewController?

Returns the child view controller that contains the source of the unwind segue.

func canPerformUnwindSegueAction(Selector, from: UIViewController, sender: Any?) -> Bool

Called on a view controller to determine whether it responds to an unwind action.

