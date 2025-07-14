

- AppKit
- NSTabViewController
-  tabView(\_:willSelect:) 

Instance Method

# tabView(\_:willSelect:)

Informs the tab view controller that the specified tab is about to be selected.

macOS 10.10+

``` source
@MainActor
func tabView(
    _ tabView: NSTabView,
    willSelect tabViewItem: NSTabViewItem?
)
```

## Parameters 

`tabView`  

The tab view object whose tab is about to be selected.

`tabViewItem`  

The tab view item that will be selected.

## Discussion

This method is a delegate method called by the NSTabView object when changes occur. Use it to update your UI or perform any tasks before a tab is selected.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Responding to Tab View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Asks the tab view controller if the specified tab should be selected.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab was selected.

