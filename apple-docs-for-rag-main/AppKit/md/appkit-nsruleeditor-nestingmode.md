

- AppKit
- NSRuleEditor
-  nestingMode 

Instance Property

# nestingMode

The rule editor’s nesting mode.

macOS

``` source
@MainActor
var nestingMode: NSRuleEditor.NestingMode { get set }
```

## Discussion

You typically set the nesting mode at view creation time and do not subsequently modify it. The default is `NSRuleEditorNestingModeCompound`. For a list of valid modes, see `Nesting Modes`.

## See Also

### Configuring a Rule Editor

var isEditable: Bool

A Boolean value that determines whether the rule editor is editable.

enum NestingMode

Specifies a type for nesting modes.

var canRemoveAllRows: Bool

A Boolean value that indicates whether all the rows can be removed.

var rowHeight: CGFloat

The rule editor’s row height.

