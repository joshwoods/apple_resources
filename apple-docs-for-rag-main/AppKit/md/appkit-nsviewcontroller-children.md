

- AppKit
- NSViewController
-  children 

Instance Property

# children

An array of view controllers that are hierarchical children of the view controller.

macOS 10.10+

``` source
@MainActor
var children: [NSViewController] { get set }
```

## Discussion

You can add or remove child view controllers by using this property. When you do, the addChild(_:) or removeFromParent() method gets called accordingly.

## See Also

### Managing Child View Controllers in a Custom Container

func addChild(NSViewController)

A convenience method for adding a child view controller at the end of the children array.

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

