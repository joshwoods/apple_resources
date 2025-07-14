

- UIKit
- UIViewController
-  shouldPerformSegue(withIdentifier:sender:) 

Instance Method

# shouldPerformSegue(withIdentifier:sender:)

Determines whether the segue with the specified identifier should be performed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func shouldPerformSegue(
    withIdentifier identifier: String,
    sender: Any?
) -> Bool
```

## Parameters 

`identifier`  

The string that identifies the triggered segue. In Interface Builder, you specify the segue’s identifier string in the attributes inspector. This string is used only for locating the segue inside the storyboard.

`sender`  

The object that initiated the segue. This object is made available for informational purposes during the actual segue.

## Return Value

true if the segue should be performed or false if it should be ignored.

## Mentioned in 

Customizing the behavior of segue-based presentations

## Discussion

Subclasses can override this method and use it to perform segues conditionally based on current conditions. If you do not implement this method, all segues are performed.

## See Also

### Performing segues

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

func unwind(for: UIStoryboardSegue, towards: UIViewController)

Called when an unwind segue transitions to a new view controller.

