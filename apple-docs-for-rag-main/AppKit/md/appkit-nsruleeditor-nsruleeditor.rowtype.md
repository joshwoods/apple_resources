

- AppKit
- NSRuleEditor
-  NSRuleEditor.RowType 

Enumeration

# NSRuleEditor.RowType

Specifies a type for row types.

macOS

``` source
enum RowType
```

## Overview

See `Row Types` for possible values.

## Topics

### Enumeration Cases

case compound

Specifies a compound row.

case simple

Specifies a simple row.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Obtaining Row Information

var numberOfRows: Int

The number of rows in the rule editor.

func parentRow(forRow: Int) -> Int

Returns the index of the parent of a given row.

func row(forDisplayValue: Any) -> Int

Returns the index of the row containing a given value.

func rowType(forRow: Int) -> NSRuleEditor.RowType

Returns the type of a given row.

func subrowIndexes(forRow: Int) -> IndexSet

Returns the immediate subrows of a given row.

