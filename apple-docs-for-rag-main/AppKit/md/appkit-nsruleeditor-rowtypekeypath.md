

- AppKit
- NSRuleEditor
-  rowTypeKeyPath 

Instance Property

# rowTypeKeyPath

The key path for the row type.

macOS

``` source
@MainActor
var rowTypeKeyPath: String { get set }
```

## Discussion

The key path is used to get the row type in the “rows” binding. The corresponding property should be a number that specifies an `NSRuleEditorRowType` value (see `Row Types`).

The default value is `@"rowType"`.

## See Also

### Supporting Bindings

var rowClass: AnyClass

The class used to create a new row in the “rows” binding.

var subrowsKeyPath: String

The key path for the subrows.

var criteriaKeyPath: String

The criteria key path.

var displayValuesKeyPath: String

The display values key path.

