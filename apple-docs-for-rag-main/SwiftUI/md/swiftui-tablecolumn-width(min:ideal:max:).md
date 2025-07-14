

- SwiftUI
- TableColumn
-  width(min:ideal:max:) 

Instance Method

# width(min:ideal:max:)

Creates a resizable table column with the provided constraints.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
func width(
    min: CGFloat? = nil,
    ideal: CGFloat? = nil,
    max: CGFloat? = nil
) -> TableColumn
```

Available when `RowValue` conforms to `Identifiable`, `Sort` conforms to `SortComparator`, `Content` conforms to `View`, and `Label` conforms to `View`.

## Parameters 

`min`  

The minimum width of a resizable column. If non-`nil`, the value must be greater than or equal to `0`.

`ideal`  

The ideal width of the column, used to determine the initial width of the table column. The column always starts at least as large as the set ideal size, but may be larger if table was sized larger than the ideal of all of its columns.

`max`  

The maximum width of a resizable column. If non-`nil`, the value must be greater than `0`. Pass doc://com.apple.documentation/documentation/CoreFoundation/CGFloat/1454161-infinity to indicate unconstrained maximum width.

## Discussion

Always specify at least one width constraint when calling this method. Pass `nil` or leave out a constraint to indicate no change to the sizing of a column.

To create a fixed size column use width(_:) instead.

## See Also

### Setting the column width

func width(CGFloat?) -> TableColumn&lt;RowValue, Sort, Content, Label>

Creates a fixed width table column that isn’t user resizable.

func width() -> TableColumn&lt;RowValue, Sort, Content, Label>

Sets the column’s width.

Deprecated

