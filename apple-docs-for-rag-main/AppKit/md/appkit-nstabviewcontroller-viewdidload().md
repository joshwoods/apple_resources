

- AppKit
- NSTabViewController
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

The tab view controller overrides this method and uses it to configure and layout the tab view and its contents. You can override it in your own subclasses to perform any custom initialization. For example, to replace the default tab view, override this method and set the value of the tabView property before calling `super`.

If you override this method, you must call `super` in your implementation.

## See Also

### Responding to Tab View Events

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Asks the tab view controller if the specified tab should be selected.

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab is about to be selected.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab was selected.

