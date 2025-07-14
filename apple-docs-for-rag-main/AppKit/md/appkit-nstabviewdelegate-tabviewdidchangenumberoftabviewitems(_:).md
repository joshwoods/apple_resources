

- AppKit
- NSTabViewDelegate
-  tabViewDidChangeNumberOfTabViewItems(\_:) 

Instance Method

# tabViewDidChangeNumberOfTabViewItems(\_:)

Informs the delegate that the number of tab view items in `tabView` has changed.

macOS

``` source
@MainActor
optional func tabViewDidChangeNumberOfTabViewItems(_ tabView: NSTabView)
```

## Parameters 

`tabView`  

The tab view that added or removed tabview items.

## See Also

### Related Documentation

Tab View Programming Topics

var numberOfTabViewItems: Int

The number of items in the tab view’s array of tab view items.

