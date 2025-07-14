

- AppKit
- NSTextTable
-  hidesEmptyCells 

Instance Property

# hidesEmptyCells

A Boolean value indicating whether the text table hides empty cells.

macOS

``` source
var hidesEmptyCells: Bool { get set }
```

## Discussion

The value of this property is true when the text table hides empty cells. If empty cells are hidden, locations with empty cells allow the background of the enclosing block or text container to show through.

