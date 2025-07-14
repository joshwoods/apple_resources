

- AppKit
- NSViewController
-  addChild(\_:) 

Instance Method

# addChild(\_:)

A convenience method for adding a child view controller at the end of the children array.

macOS 10.10+

``` source
@MainActor
func addChild(_ childViewController: NSViewController)
```

## Parameters 

`childViewController`  

The view controller to be added to the end of the children array.

## See Also

### Managing Child View Controllers in a Custom Container

var children: [NSViewController]

An array of view controllers that are hierarchical children of the view controller.

func transition(from: NSViewController, to: NSViewController, options: NSViewController.TransitionOptions, completionHandler: (() -> Void)?)

Performs a transition between two sibling child view controllers of the view controller.

func insertChild(NSViewController, at: Int)

Inserts a specified child view controller into the children array at a specified position.

func removeChild(at: Int)

Removes a specified child controller from the view controller.

func removeFromParent()

Removes the called view controller from its parent view controller.

func preferredContentSizeDidChange(for: NSViewController)

Called when there is a change in value of the preferredContentSize property of a child view controller or a presented view controller.

