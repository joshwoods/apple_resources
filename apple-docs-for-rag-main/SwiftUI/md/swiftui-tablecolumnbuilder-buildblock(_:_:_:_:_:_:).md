

- SwiftUI
- TableColumnBuilder
-  buildBlock(\_:\_:\_:\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:\_:\_:\_:)

Creates an unsortable column result from six sources.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
static func buildBlock(
    _ c0: C0,
    _ c1: C1,
    _ c2: C2,
    _ c3: C3,
    _ c4: C4,
    _ c5: C5
) -> TupleTableColumnContent where RowValue == C0.TableRowValue, C0 : TableColumnContent, C1 : TableColumnContent, C2 : TableColumnContent, C3 : TableColumnContent, C4 : TableColumnContent, C5 : TableColumnContent, C0.TableColumnSortComparator == Never, C0.TableRowValue == C1.TableRowValue, C1.TableColumnSortComparator == Never, C1.TableRowValue == C2.TableRowValue, C2.TableColumnSortComparator == Never, C2.TableRowValue == C3.TableRowValue, C3.TableColumnSortComparator == Never, C3.TableRowValue == C4.TableRowValue, C4.TableColumnSortComparator == Never, C4.TableRowValue == C5.TableRowValue, C5.TableColumnSortComparator == Never
```

Available when `RowValue` conforms to `Identifiable` and `Sort` conforms to `SortComparator`.

Show all declarations

## See Also

### Building a column

static buildBlock(_:)

Creates a single, unsortable column result.

static buildBlock(_:_:)

Creates an unsortable column result from two sources.

static buildBlock(_:_:_:)

Creates an unsortable column result from three sources.

static buildBlock(_:_:_:_:)

Creates an unsortable column result from four sources.

static buildBlock(_:_:_:_:_:)

Creates an unsortable column result from five sources.

static buildBlock(_:_:_:_:_:_:_:)

Creates an unsortable column result from seven sources.

static buildBlock(_:_:_:_:_:_:_:_:)

Creates an unsortable column result from eight sources.

static buildBlock(_:_:_:_:_:_:_:_:_:)

Creates an unsortable column result from nine sources.

static buildBlock(_:_:_:_:_:_:_:_:_:_:)

Creates an unsortable column result from ten sources.

static buildExpression(_:)

Creates a generic, unsortable single column expression.

