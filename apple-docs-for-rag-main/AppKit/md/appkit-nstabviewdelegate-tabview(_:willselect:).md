

- AppKit
- NSTabViewDelegate
-  tabView(\_:willSelect:) 

Instance Method

# tabView(\_:willSelect:)

Informs the delegate that `tabView` is about to select `tabViewItem`.

macOS

``` source
@MainActor
optional func tabView(
    _ tabView: NSTabView,
    willSelect tabViewItem: NSTabViewItem?
)
```

## Parameters 

`tabView`  

The tab view that sent the request.

`tabViewItem`  

The tab view item that is about to be selected.

## See Also

### Selecting a Tab

func tabView(NSTabView, shouldSelect: NSTabViewItem?) -> Bool

Invoked just before `tabViewItem` in `tabView` is selected.

func tabView(NSTabView, didSelect: NSTabViewItem?)

Informs the delegate that `tabView` has selected `tabViewItem`.

