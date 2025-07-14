

- UIKit
- UIViewController
-  allowedChildrenForUnwinding(from:) 

Instance Method

# allowedChildrenForUnwinding(from:)

Returns an array of child view controllers to search for an unwind segue destination.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0–1.0Deprecated

``` source
@MainActor
func allowedChildrenForUnwinding(from source: UIStoryboardUnwindSegueSource) -> [UIViewController]
```

## Parameters 

`source`  

The unwind segue source object containing information about the unwind segue.

## Return Value

An array of view controllers representing the child view controllers to search. The order of the items in the array determines the search order.

## Mentioned in 

Creating a custom container view controller

## Discussion

UIKit calls this method when searching for the destination of an unwind segue. The default implementation returns the contents of the children property minus the view controller returned by the childContaining(_:) method. You can override this method as needed in your custom container view controllers to change the search order. For example, a navigation controller reverses the order so that the search starts with the view controller at the top of the navigation stack.

## See Also

### Performing segues

func shouldPerformSegue(withIdentifier: String, sender: Any?) -> Bool

Determines whether the segue with the specified identifier should be performed.

func prepare(for: UIStoryboardSegue, sender: Any?)

Notifies the view controller that a segue is about to be performed.

func performSegue(withIdentifier: String, sender: Any?)

Initiates the segue with the specified identifier from the current view controller’s storyboard file.

func childContaining(UIStoryboardUnwindSegueSource) -> UIViewController?

Returns the child view controller that contains the source of the unwind segue.

func canPerformUnwindSegueAction(Selector, from: UIViewController, sender: Any?) -> Bool

Called on a view controller to determine whether it responds to an unwind action.

func unwind(for: UIStoryboardSegue, towards: UIViewController)

Called when an unwind segue transitions to a new view controller.

