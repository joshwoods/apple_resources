

- AppKit
- NSTabViewController
-  tabView(\_:didSelect:) 

Instance Method

# tabView(\_:didSelect:)

Informs the tab view controller that the specified tab was selected.

macOS 10.10+

``` source
@MainActor
func tabView(
    _ tabView: NSTabView,
    didSelect tabViewItem: NSTabViewItem?
)
```

## Parameters 

`tabView`  

The tab view object whose tab was selected.

`tabViewItem`  

The tab view item that was selected.

## Discussion

This method is a delegate method called by the NSTabView object when changes occur. Use it to perform any necessary tasks after a tab is selected.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Responding to Tab View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Asks the tab view controller if the specified tab should be selected.

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab is about to be selected.

