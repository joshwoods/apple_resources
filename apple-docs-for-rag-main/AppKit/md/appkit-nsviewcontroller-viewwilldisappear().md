

- AppKit
- NSViewController
-  viewWillDisappear() 

Instance Method

# viewWillDisappear()

Called when the view controller’s view is about to be removed from the view hierarchy in the window.

macOS 10.10+

``` source
@MainActor
func viewWillDisappear()
```

## Discussion

You can override this method to perform tasks that are to precede the disappearance of the view controller’s view, such as stopping a continuous animation that you started in response to the viewDidAppear() method call. This method is called when:

- The view is about to be removed from the view hierarchy of the window

- The view is about to be hidden or obscured, such as in the case of a view controller whose parent is a tab view controller and the user switched to another tab

- The window is being closed

If you override this method, call this method on `super` at some point in your implementation in case a superclass also overrides this method.

The default implementation of this method does nothing.

## See Also

### Responding to View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

func loadViewIfNeeded()

var isViewLoaded: Bool

A Boolean value indicating whether the view controller’s view is loaded into memory.

var viewIfLoaded: NSView?

func viewWillAppear()

Called after the view controller’s view has been loaded into memory is about to be added to the view hierarchy in the window.

func viewDidAppear()

Called when the view controller’s view is fully transitioned onto the screen.

func viewDidDisappear()

Called after the view controller’s view is removed from the view hierarchy in a window.

