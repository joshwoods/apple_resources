

- AppKit
- NSViewController
-  removeFromParent() 

Instance Method

# removeFromParent()

Removes the called view controller from its parent view controller.

macOS 10.10+

``` source
@MainActor
func removeFromParent()
```

## Discussion

Use this method to remove a child view controller from its parent view controller, unless you want to perform work during the removal. In that case, instead override the removeChild(at:) method to perform that work and call that method.

This is a convenience method that calls the removeChild(at:) method, automatically supplying the appropriate index value as an argument.

## See Also

### Managing Child View Controllers in a Custom Container

func addChild(NSViewController)

A convenience method for adding a child view controller at the end of the children array.

var children: [NSViewController]

An array of view controllers that are hierarchical children of the view controller.

func transition(from: NSViewController, to: NSViewController, options: NSViewController.TransitionOptions, completionHandler: (() -> Void)?)

Performs a transition between two sibling child view controllers of the view controller.

func insertChild(NSViewController, at: Int)

Inserts a specified child view controller into the children array at a specified position.

func removeChild(at: Int)

Removes a specified child controller from the view controller.

func preferredContentSizeDidChange(for: NSViewController)

Called when there is a change in value of the preferredContentSize property of a child view controller or a presented view controller.

