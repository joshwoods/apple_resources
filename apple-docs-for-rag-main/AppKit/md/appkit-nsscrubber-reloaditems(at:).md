

- AppKit
- NSScrubber
-  reloadItems(at:) 

Instance Method

# reloadItems(at:)

Reloads the items at the specified indexes.

macOS 10.12.2+

``` source
@MainActor
func reloadItems(at indexes: IndexSet)
```

## Parameters 

`indexes`  

The indexes of the items to reload, provided in an index set (IndexSet).

## Discussion

The scrubber makes requests for updated views from the data source and then animates their display.

## See Also

### Reloading content

func reloadData()

Reloads the content of the entire scrubber, and deselects the currently selected item.

