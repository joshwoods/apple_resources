

- AppKit
- NSTableColumn
-  sortDescriptorPrototype 

Instance Property

# sortDescriptorPrototype

The table column’s sort descriptor prototype.

macOS

``` source
@NSCopying @MainActor
var sortDescriptorPrototype: NSSortDescriptor? { get set }
```

## Discussion

A table column is considered sortable if it has a sort descriptor that specifies the sorting direction, a key to sort by, and a selector that defines how to sort.

