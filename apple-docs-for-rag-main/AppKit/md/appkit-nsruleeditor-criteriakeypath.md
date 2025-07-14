

- AppKit
- NSRuleEditor
-  criteriaKeyPath 

Instance Property

# criteriaKeyPath

The criteria key path.

macOS

``` source
@MainActor
var criteriaKeyPath: String { get set }
```

## Discussion

The key path is used to get the criteria for a row in the “rows” binding. The criteria objects are the objects returned by calling the delegate’s ruleEditor(_:child:forCriterion:with:) method once for every child in the specified row. The corresponding property is an ordered to-many relationship.

The default value is `@"criteria"`.

## See Also

### Supporting Bindings

var rowClass: AnyClass

The class used to create a new row in the “rows” binding.

var rowTypeKeyPath: String

The key path for the row type.

var subrowsKeyPath: String

The key path for the subrows.

var displayValuesKeyPath: String

The display values key path.

