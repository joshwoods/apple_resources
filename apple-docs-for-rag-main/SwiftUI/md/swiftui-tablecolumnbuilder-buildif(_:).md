

- SwiftUI
- TableColumnBuilder
-  buildIf(\_:) 

Type Method

# buildIf(\_:)

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+visionOS 1.1+

``` source
static func buildIf(_ content: C?) -> C? where RowValue == C.TableRowValue, C : TableColumnContent, C.TableColumnSortComparator == Never
```

Available when `RowValue` conforms to `Identifiable` and `Sort` conforms to `SortComparator`.

Show all declarations

