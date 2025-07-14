

- AppKit
- NSRuleEditor
-  displayValuesKeyPath 

Instance Property

# displayValuesKeyPath

The display values key path.

macOS

``` source
@MainActor
var displayValuesKeyPath: String { get set }
```

## Discussion

The key path is used to get the display values for a row in the “rows” binding. The display values are the objects returned by calling the delegate’s ruleEditor(_:displayValueForCriterion:inRow:) method for the specified row. The corresponding property is an ordered to-many relationship.

The default is `@"displayValues"`.

## See Also

### Supporting Bindings

var rowClass: AnyClass

The class used to create a new row in the “rows” binding.

var rowTypeKeyPath: String

The key path for the row type.

var subrowsKeyPath: String

The key path for the subrows.

var criteriaKeyPath: String

The criteria key path.

