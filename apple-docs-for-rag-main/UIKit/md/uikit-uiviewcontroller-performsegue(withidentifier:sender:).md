

- UIKit
- UIViewController
-  performSegue(withIdentifier:sender:) 

Instance Method

# performSegue(withIdentifier:sender:)

Initiates the segue with the specified identifier from the current view controller’s storyboard file.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func performSegue(
    withIdentifier identifier: String,
    sender: Any?
)
```

## Parameters 

`identifier`  

The string that identifies the triggered segue. In Interface Builder, you specify the segue’s identifier string in the attributes inspector.

This method throws an Exception handling if there is no segue with the specified identifier.

`sender`  

The object that you want to use to initiate the segue. This object is made available for informational purposes during the actual segue.

## Discussion

Normally, segues are initiated automatically and not using this method. However, you can use this method in cases where the segue could not be configured in your storyboard file. For example, you might call it from a custom action handler used in response to shake or accelerometer events.

The current view controller must have been loaded from a storyboard. If its storyboard property is `nil`, perhaps because you allocated and initialized the view controller yourself, this method throws an exception.

## See Also

### Performing segues

func shouldPerformSegue(withIdentifier: String, sender: Any?) -> Bool

Determines whether the segue with the specified identifier should be performed.

func prepare(for: UIStoryboardSegue, sender: Any?)

Notifies the view controller that a segue is about to be performed.

func allowedChildrenForUnwinding(from: UIStoryboardUnwindSegueSource) -> [UIViewController]

Returns an array of child view controllers to search for an unwind segue destination.

func childContaining(UIStoryboardUnwindSegueSource) -> UIViewController?

Returns the child view controller that contains the source of the unwind segue.

func canPerformUnwindSegueAction(Selector, from: UIViewController, sender: Any?) -> Bool

Called on a view controller to determine whether it responds to an unwind action.

func unwind(for: UIStoryboardSegue, towards: UIViewController)

Called when an unwind segue transitions to a new view controller.

