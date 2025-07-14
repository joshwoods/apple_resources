

- AppKit
- NSViewController
-  viewDidAppear() 

Instance Method

# viewDidAppear()

Called when the view controller’s view is fully transitioned onto the screen.

macOS 10.10+

``` source
@MainActor
func viewDidAppear()
```

## Discussion

This method is called after the completion of any drawing and animations involved in the initial appearance of the view. You can override this method to perform tasks appropriate for that time, such as work that should not interfere with the presentation animation, or starting an animation that you want to begin after the view appears.

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

func viewWillDisappear()

Called when the view controller’s view is about to be removed from the view hierarchy in the window.

func viewDidDisappear()

Called after the view controller’s view is removed from the view hierarchy in a window.

