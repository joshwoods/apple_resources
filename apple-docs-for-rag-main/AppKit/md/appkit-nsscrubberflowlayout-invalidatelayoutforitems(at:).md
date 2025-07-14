

- AppKit
- NSScrubberFlowLayout
-  invalidateLayoutForItems(at:) 

Instance Method

# invalidateLayoutForItems(at:)

Informs the scrubber that it should perform a new layout pass for the items at the specified indexes.

macOS 10.12.2+

``` source
@MainActor
func invalidateLayoutForItems(at invalidItemIndexes: IndexSet)
```

## Parameters 

`invalidItemIndexes`  

An index set containing the indexes of the items whose layout should be invalidated.

