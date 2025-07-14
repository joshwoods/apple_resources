

- AppKit
- NSTableColumn
-  isHidden 

Instance Property

# isHidden

A Boolean that indicates whether the table column is hidden.

macOS 10.5+

``` source
@MainActor
var isHidden: Bool { get set }
```

## Discussion

When the value of this property is true, the table column is hidden. The default value is false.

Columns that are hidden still exist in the table view object’s tableColumns array and are included in the table view’s numberOfColumns count.

The hidden state is stored when the table view autosaves the table column state.

