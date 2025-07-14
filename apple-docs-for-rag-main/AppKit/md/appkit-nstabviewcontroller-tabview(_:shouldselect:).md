

- AppKit
- NSTabViewController
-  tabView(\_:shouldSelect:) 

Instance Method

# tabView(\_:shouldSelect:)

Asks the tab view controller if the specified tab should be selected.

macOS 10.10+

``` source
@MainActor
func tabView(
    _ tabView: NSTabView,
    shouldSelect tabViewItem: NSTabViewItem?
) -> Bool
```

## Parameters 

`tabView`  

The tab view object making the request.

`tabViewItem`  

The tab view item to select.

## Return Value

true if the tab should be selected or false if it should not be selected.

## Discussion

This method is a delegate method called by the NSTabView object when changes occur. Use it to dynamically determine whether a tab should be selected.

If you override this method, you must call `super` at some point in your implementation.

## See Also

### Responding to Tab View Events

func viewDidLoad()

Called after the view controller’s view has been loaded into memory.

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab is about to be selected.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the tab view controller that the specified tab was selected.

