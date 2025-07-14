

- AppKit
- NSStatusBar
-  removeStatusItem(\_:) 

Instance Method

# removeStatusItem(\_:)

Removes the specified status item from the receiver.

macOS

``` source
func removeStatusItem(_ item: NSStatusItem)
```

## Parameters 

`item`  

The `NSStatusItem` object to remove.

## Discussion

Status items to the left of the specified one in the status bar shift to the right to reclaim its space.

## See Also

### Managing Status items

func statusItem(withLength: CGFloat) -> NSStatusItem

Returns a newly created status item that has been allotted a specified space within the status bar.

