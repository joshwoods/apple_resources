

- AppKit
- NSRuleEditor
-  NSRuleEditor.NestingMode 

Enumeration

# NSRuleEditor.NestingMode

Specifies a type for nesting modes.

macOS

``` source
enum NestingMode
```

## Overview

See `Nesting Modes` for possible values.

## Topics

### Modes

case compound

Unlimited nesting and compound rows.

case list

Allows a single list, with no nesting and no compound rows.

case simple

One compound row at the top with subrows beneath it, and no further nesting allowed.

case single

Only a single row is allowed.

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

### Configuring a Rule Editor

var isEditable: Bool

A Boolean value that determines whether the rule editor is editable.

var nestingMode: NSRuleEditor.NestingMode

The rule editor’s nesting mode.

var canRemoveAllRows: Bool

A Boolean value that indicates whether all the rows can be removed.

var rowHeight: CGFloat

The rule editor’s row height.

