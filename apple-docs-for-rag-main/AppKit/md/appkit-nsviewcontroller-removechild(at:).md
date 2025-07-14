

- AppKit
- NSViewController
-  removeChild(at:) 

Instance Method

# removeChild(at:)

Removes a specified child controller from the view controller.

macOS 10.10+

``` source
@MainActor
func removeChild(at index: Int)
```

## Parameters 

`index`  

The index in the children array for the child view controller you want to remove.

## Discussion

Override this method if you want to perform work during the removal of a child view controller. If you do override this method, in your implementation call this method on `super`.

If you just want to remove a child view controller, instead use the removeFromParent() method

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

func removeFromParent()

Removes the called view controller from its parent view controller.

func preferredContentSizeDidChange(for: NSViewController)

Called when there is a change in value of the preferredContentSize property of a child view controller or a presented view controller.

