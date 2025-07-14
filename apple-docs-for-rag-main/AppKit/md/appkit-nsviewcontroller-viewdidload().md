

- AppKit
- NSViewController
-  viewDidLoad() 

Instance Method

# viewDidLoad()

Called after the view controller’s view has been loaded into memory.

macOS 10.10+

``` source
@MainActor
func viewDidLoad()
```

## Discussion

You can override this method to perform tasks to immediately follow the setting of the view property.

Typically, your override would perform one-time instantiation and initialization of the contents of the view controller’s view. If you override this method, call this method on `super` at some point in your implementation in case a superclass also overrides this method.

For a view controller originating in a nib file, this method is called immediately after the view property is set. For a view controller created programmatically, this method is called immediately after the loadView() method completes.

The default implementation of this method does nothing.

## See Also

### Responding to View Events

func loadViewIfNeeded()

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

