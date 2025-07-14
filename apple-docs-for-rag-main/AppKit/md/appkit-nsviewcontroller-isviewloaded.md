

- AppKit
- NSViewController
-  isViewLoaded 

Instance Property

# isViewLoaded

A Boolean value indicating whether the view controller’s view is loaded into memory.

macOS 10.10+

``` source
@MainActor
var isViewLoaded: Bool { get }
```

## See Also

### Responding to View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

func loadViewIfNeeded()

var viewIfLoaded: NSView?

func viewWillAppear()

Called after the view controller’s view has been loaded into memory is about to be added to the view hierarchy in the window.

func viewDidAppear()

Called when the view controller’s view is fully transitioned onto the screen.

func viewWillDisappear()

Called when the view controller’s view is about to be removed from the view hierarchy in the window.

func viewDidDisappear()

Called after the view controller’s view is removed from the view hierarchy in a window.

