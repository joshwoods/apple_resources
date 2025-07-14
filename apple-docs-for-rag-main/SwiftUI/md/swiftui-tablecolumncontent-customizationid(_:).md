

- SwiftUI
- TableColumnContent
-  customizationID(\_:) 

Instance Method

# customizationID(\_:)

Sets the identifier to be associated with a column when persisting its state with `TableColumnCustomization`.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func customizationID(_ id: String) -> some TableColumnContent
```

## Parameters 

`id`  

The identifier to associate with a column.

## Discussion

This is required to allow user customization of a specific table column, in addition to the table as a whole being provided a binding to a `TableColumnCustomization`.

The identifier needs to to be stable, including across app version updates, since it is used to persist the user customization.

## See Also

### Configuring the content

func alignment(TableColumnAlignment) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the alignment of the column, applying to both its column header label and the row view content for that column.

func defaultVisibility(Visibility) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the default visibility of a table column.

func disabledCustomizationBehavior(TableColumnCustomizationBehavior) -> some TableColumnContent&lt;Self.TableRowValue, Self.TableColumnSortComparator> 

Sets the disabled customization behavior for a table column.

