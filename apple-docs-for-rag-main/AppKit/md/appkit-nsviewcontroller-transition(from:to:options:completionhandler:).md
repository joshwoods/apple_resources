

- AppKit
- NSViewController
-  transition(from:to:options:completionHandler:) 

Instance Method

# transition(from:to:options:completionHandler:)

Performs a transition between two sibling child view controllers of the view controller.

macOS 10.10+

``` source
@MainActor
func transition(
    from fromViewController: NSViewController,
    to toViewController: NSViewController,
    options: NSViewController.TransitionOptions = [],
    completionHandler completion: (() -> Void)? = nil
)
```

``` source
@MainActor
func transition(
    from fromViewController: NSViewController,
    to toViewController: NSViewController,
    options: NSViewController.TransitionOptions = []
) async
```

## Parameters 

`fromViewController`  

A child view controller whose view is visible in the view controller’s view hierarchy.

Note

The view of this view controller must have a superview, or else this method raises an exception.

`toViewController`  

A child view controller whose view is not in the view controller’s view hierarchy.

`options`  

A bitmask of options that specify how you want to perform the transition animation. For the options, see the NSViewController.TransitionOptions enumeration.

`completion`  

A block called immediately after the transition animation completes.

## Discussion

Use this method to transition between sibling child view controllers owned by a parent view controller (which is the receiver of this method).

This method adds the view in the `toViewController` view controller to the superview of the view in the `fromViewController` view controller. Likewise, this method removes the `fromViewController` view from the parent view controller’s view hierarchy at the appropriate time. It is important to allow this method to add and remove these views.

Note

The receiver of this method must be the parent view controller of the `fromViewController` and `toViewController` view controllers, or else this method raises an exception.

To create a parent/child relationship between view controllers, use the addChild(_:) method or the insertChild(_:at:) method.

## See Also

### Managing Child View Controllers in a Custom Container

func addChild(NSViewController)

A convenience method for adding a child view controller at the end of the children array.

var children: [NSViewController]

An array of view controllers that are hierarchical children of the view controller.

func insertChild(NSViewController, at: Int)

Inserts a specified child view controller into the children array at a specified position.

func removeChild(at: Int)

Removes a specified child controller from the view controller.

func removeFromParent()

Removes the called view controller from its parent view controller.

func preferredContentSizeDidChange(for: NSViewController)

Called when there is a change in value of the preferredContentSize property of a child view controller or a presented view controller.

