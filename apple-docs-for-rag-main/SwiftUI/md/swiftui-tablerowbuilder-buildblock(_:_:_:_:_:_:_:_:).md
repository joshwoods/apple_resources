

- SwiftUI
- TableRowBuilder
-  buildBlock(\_:\_:\_:\_:\_:\_:\_:\_:) 

Type Method

# buildBlock(\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a row result from eight sources.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
static func buildBlock(
    _ c0: C0,
    _ c1: C1,
    _ c2: C2,
    _ c3: C3,
    _ c4: C4,
    _ c5: C5,
    _ c6: C6,
    _ c7: C7
) -> TupleTableRowContent where Value == C0.TableRowValue, C0 : TableRowContent, C1 : TableRowContent, C2 : TableRowContent, C3 : TableRowContent, C4 : TableRowContent, C5 : TableRowContent, C6 : TableRowContent, C7 : TableRowContent, C0.TableRowValue == C1.TableRowValue, C1.TableRowValue == C2.TableRowValue, C2.TableRowValue == C3.TableRowValue, C3.TableRowValue == C4.TableRowValue, C4.TableRowValue == C5.TableRowValue, C5.TableRowValue == C6.TableRowValue, C6.TableRowValue == C7.TableRowValue
```

Available when `Value` conforms to `Identifiable`.

## See Also

### Building a row from sources

static func buildBlock&lt;C>(C) -> C

Creates a single row result.

static func buildBlock&lt;C0, C1>(C0, C1) -> TupleTableRowContent&lt;Value, (C0, C1)>

Creates a row result from two sources.

static func buildBlock&lt;C0, C1, C2>(C0, C1, C2) -> TupleTableRowContent&lt;Value, (C0, C1, C2)>

Creates a row result from three sources.

static func buildBlock&lt;C0, C1, C2, C3>(C0, C1, C2, C3) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3)>

Creates a row result from four sources.

static func buildBlock&lt;C0, C1, C2, C3, C4>(C0, C1, C2, C3, C4) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4)>

Creates a row result from five sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5>(C0, C1, C2, C3, C4, C5) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5)>

Creates a row result from six sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6>(C0, C1, C2, C3, C4, C5, C6) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6)>

Creates a row result from seven sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8)>

Creates a row result from nine sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

Creates a row result from ten sources.

