

- UIKit
- UIViewController
-  childContaining(\_:) 

Instance Method

# childContaining(\_:)

Returns the child view controller that contains the source of the unwind segue.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0–1.0Deprecated

``` source
@MainActor
func childContaining(_ source: UIStoryboardUnwindSegueSource) -> UIViewController?
```

## Parameters 

`source`  

The unwind segue source object containing information about the unwind segue.

## Return Value

The view controller that contains the segue source.

## Discussion

Container view controllers call this method to identify the child view controller that is the source of the unwind segue. Typically, you call this method from your allowedChildrenForUnwinding(from:) method so that you can remove the corresponding view controller from the returned list of children.

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

func canPerformUnwindSegueAction(Selector, from: UIViewController, sender: Any?) -> Bool

Called on a view controller to determine whether it responds to an unwind action.

func unwind(for: UIStoryboardSegue, towards: UIViewController)

Called when an unwind segue transitions to a new view controller.

