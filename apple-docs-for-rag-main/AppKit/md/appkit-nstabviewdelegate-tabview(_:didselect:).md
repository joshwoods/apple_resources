

- AppKit
- NSTabViewDelegate
-  tabView(\_:didSelect:) 

Instance Method

# tabView(\_:didSelect:)

Informs the delegate that `tabView` has selected `tabViewItem`.

macOS

``` source
@MainActor
optional func tabView(
    _ tabView: NSTabView,
    didSelect tabViewItem: NSTabViewItem?
)
```

## Parameters 

`tabView`  

The tab view that sent the request.

`tabViewItem`  

The tab view item that was selected.

## See Also

### Selecting a Tab

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Invoked just before `tabViewItem` in `tabView` is selected.

func tabView(NSTabView, willSelect: NSTabViewItem?)

Informs the delegate that `tabView` is about to select `tabViewItem`.

