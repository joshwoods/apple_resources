

- AppKit
- NSTabViewDelegate
-  tabView(\_:shouldSelect:) 

Instance Method

# tabView(\_:shouldSelect:)

Invoked just before `tabViewItem` in `tabView` is selected.

macOS

``` source
@MainActor
optional func tabView(
    _ tabView: NSTabView,
    shouldSelect tabViewItem: NSTabViewItem?
) -> Bool
```

## Parameters 

`tabView`  

The tab view that sent the request.

`tabViewItem`  

The tab view item to select.

## Return Value

true if the tab view item should be selected, otherwise false.

## See Also

### Selecting a Tab

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the delegate that `tabView` is about to select `tabViewItem`.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the delegate that `tabView` has selected `tabViewItem`.

