

- SwiftUI
- TableColumnContent
-  alignment(\_:) 

Instance Method

# alignment(\_:)

Sets the alignment of the column, applying to both its column header label and the row view content for that column.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func alignment(_ alignment: TableColumnAlignment) -> some TableColumnContent
```

## Parameters 

`alignment`  

The alignment to apply to the column.

## See Also

### Configuring the content

func customizationID(String) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the identifier to be associated with a column when persisting its state with `TableColumnCustomization`.

func defaultVisibility(Visibility) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the default visibility of a table column.

func disabledCustomizationBehavior(TableColumnCustomizationBehavior) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the disabled customization behavior for a table column.

