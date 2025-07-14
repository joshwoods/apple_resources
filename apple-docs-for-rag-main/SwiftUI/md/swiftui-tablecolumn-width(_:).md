

- SwiftUI
- TableColumn
-  width(\_:) 

Instance Method

# width(\_:)

Creates a fixed width table column that isn’t user resizable.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
func width(_ width: CGFloat? = nil) -> TableColumn
```

Available when `RowValue` conforms to `Identifiable`, `Sort` conforms to `SortComparator`, `Content` conforms to `View`, and `Label` conforms to `View`.

## Parameters 

`width`  

A fixed width for the resulting column. If `width` is `nil`, the resulting column has no change in sizing.

## See Also

### Setting the column width

func width(min: CGFloat?, ideal: CGFloat?, max: CGFloat?) -> TableColumn&lt;RowValue, Sort, Content, Label>

Creates a resizable table column with the provided constraints.

func width() -> TableColumn&lt;RowValue, Sort, Content, Label>

Sets the column’s width.

Deprecated

