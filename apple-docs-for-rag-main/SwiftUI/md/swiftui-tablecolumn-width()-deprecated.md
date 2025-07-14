

- SwiftUI
- TableColumn
-  width() Deprecated

Instance Method

# width()

Sets the column’s width.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
func width() -> TableColumn
```

Available when `RowValue` conforms to `Identifiable`, `Sort` conforms to `SortComparator`, `Content` conforms to `View`, and `Label` conforms to `View`.

Deprecated

Use width(_:) or width(min:ideal:max:) instead.

## See Also

### Setting the column width

func width(CGFloat?) -> TableColumn&lt;RowValue, Sort, Content, Label>

Creates a fixed width table column that isn’t user resizable.

func width(min: CGFloat?, ideal: CGFloat?, max: CGFloat?) -> TableColumn&lt;RowValue, Sort, Content, Label>

Creates a resizable table column with the provided constraints.

