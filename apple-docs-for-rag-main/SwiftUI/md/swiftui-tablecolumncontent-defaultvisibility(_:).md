

- SwiftUI
- TableColumnContent
-  defaultVisibility(\_:) 

Instance Method

# defaultVisibility(\_:)

Sets the default visibility of a table column.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func defaultVisibility(_ visibility: Visibility) -> some TableColumnContent
```

## Parameters 

`visibility`  

The default visibility to apply to columns.

## Discussion

A `hidden` column will not be visible, unless the `Table` is also bound to `TableColumnCustomization` and either modified programmatically or by the user.

## See Also

### Configuring the content

func alignment(TableColumnAlignment) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the alignment of the column, applying to both its column header label and the row view content for that column.

func customizationID(String) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the identifier to be associated with a column when persisting its state with `TableColumnCustomization`.

func disabledCustomizationBehavior(TableColumnCustomizationBehavior) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the disabled customization behavior for a table column.

