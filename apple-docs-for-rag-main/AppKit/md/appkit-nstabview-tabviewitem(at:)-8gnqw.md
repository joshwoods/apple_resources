

- AppKit
- NSTabView
-  tabViewItem(at:) 

Instance Method

# tabViewItem(at:)

Returns the tab view item at the specified point.

macOS

``` source
@MainActor
func tabViewItem(at point: NSPoint) -> NSTabViewItem?
```

## Parameters 

`point`  

The hit point.

## Return Value

The tab view item under the hit point, or `nil` if no tab view item is under that location.

## Discussion

You can use this method to find a tab view item based on a user’s mouse click.

