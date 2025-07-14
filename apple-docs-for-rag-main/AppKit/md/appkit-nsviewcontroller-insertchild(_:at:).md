

- AppKit
- NSViewController
-  insertChild(\_:at:) 

Instance Method

# insertChild(\_:at:)

Inserts a specified child view controller into the children array at a specified position.

macOS 10.10+

``` source
@MainActor
func insertChild(
    _ childViewController: NSViewController,
    at index: Int
)
```

## Parameters 

`childViewController`  

The child view controller to add to the children array.

`index`  

The index in the children array at which to insert the child view controller. This value must not be greater than the count of elements in the array.

## Discussion

You should instead use the addChild(_:) method unless you want to perform work on child view controllers as you add them. In that case, override this method to perform that work.

If a child view controller has a different parent when you call this method, the child is first be removed from its existing parent by calling the child’s removeFromParent() method.

## See Also

### Managing Child View Controllers in a Custom Container

func addChild(NSViewController)

A convenience method for adding a child view controller at the end of the children array.

var children: [NSViewController]

An array of view controllers that are hierarchical children of the view controller.

func transition(from: NSViewController, to: NSViewController, options: NSViewController.TransitionOptions, completionHandler: (() -> Void)?)

Performs a transition between two sibling child view controllers of the view controller.

func removeChild(at: Int)

Removes a specified child controller from the view controller.

func removeFromParent()

Removes the called view controller from its parent view controller.

func preferredContentSizeDidChange(for: NSViewController)

Called when there is a change in value of the preferredContentSize property of a child view controller or a presented view controller.

