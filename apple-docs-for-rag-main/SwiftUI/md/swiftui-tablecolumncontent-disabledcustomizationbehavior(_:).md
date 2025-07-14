

- SwiftUI
- TableColumnContent
-  disabledCustomizationBehavior(\_:) 

Instance Method

# disabledCustomizationBehavior(\_:)

Sets the disabled customization behavior for a table column.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func disabledCustomizationBehavior(_ behavior: TableColumnCustomizationBehavior) -> some TableColumnContent
```

## Parameters 

`behavior`  

The behavior to disable, or `.all` to not allow any customization.

## Discussion

When the containing `Table` is bound to some `TableColumnCustomization`, all columns will be able to be customized by the user on macOS by default (i.e. `TableColumnCustomizationBehavior.all`). This modifier allows disabling specific behavior.

This modifier has no effect on iOS since `Table` does not support any built-in user customization features.

This does not prevent programmatic changes to a table column customization.

## See Also

### Configuring the content

func alignment(TableColumnAlignment) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the alignment of the column, applying to both its column header label and the row view content for that column.

func customizationID(String) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the identifier to be associated with a column when persisting its state with `TableColumnCustomization`.

func defaultVisibility(Visibility) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the default visibility of a table column.

