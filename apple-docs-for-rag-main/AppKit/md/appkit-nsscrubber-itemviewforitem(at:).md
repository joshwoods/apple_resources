

- AppKit
- NSScrubber
-  itemViewForItem(at:) 

Instance Method

# itemViewForItem(at:)

Returns the view for the item at the specified index.

macOS 10.12.2+

``` source
@MainActor
func itemViewForItem(at index: Int) -> NSScrubberItemView?
```

## Parameters 

`index`  

The index of the item whose view you want.

## Return Value

The view for the specified index or `nil` if the item is not currently visible.

