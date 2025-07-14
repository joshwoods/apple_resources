

- SwiftUI
- TableColumnBuilder
-  buildEither(second:) 

Type Method

# buildEither(second:)

Creates a row result for the second of two row content alternatives.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+visionOS 1.1+

``` source
static func buildEither(second: F) -> _ConditionalContent where RowValue == T.TableRowValue, Sort == T.TableColumnSortComparator, T : TableColumnContent, F : TableColumnContent, T.TableColumnSortComparator == F.TableColumnSortComparator, T.TableRowValue == F.TableRowValue
```

Available when `RowValue` conforms to `Identifiable` and `Sort` conforms to `SortComparator`.

Show all declarations

## Discussion

This method provides support for “if” statements in multi-statement closures, producing conditional content for the “else” branch.

