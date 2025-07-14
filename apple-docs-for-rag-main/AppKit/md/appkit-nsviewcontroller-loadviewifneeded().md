

- AppKit
- NSViewController
-  loadViewIfNeeded() 

Instance Method

# loadViewIfNeeded()

macOS 14.0+

``` source
@MainActor
func loadViewIfNeeded()
```

## See Also

### Responding to View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

var isViewLoaded: Bool

A Boolean value indicating whether the view controller’s view is loaded into memory.

var viewIfLoaded: NSView?

func viewWillAppear()

Called after the view controller’s view has been loaded into memory is about to be added to the view hierarchy in the window.

func viewDidAppear()

Called when the view controller’s view is fully transitioned onto the screen.

func viewWillDisappear()

Called when the view controller’s view is about to be removed from the view hierarchy in the window.

func viewDidDisappear()

Called after the view controller’s view is removed from the view hierarchy in a window.

