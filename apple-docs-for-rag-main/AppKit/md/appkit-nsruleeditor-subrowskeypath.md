

- AppKit
- NSRuleEditor
-  subrowsKeyPath 

Instance Property

# subrowsKeyPath

The key path for the subrows.

macOS

``` source
@MainActor
var subrowsKeyPath: String { get set }
```

## Discussion

The key path is used to get the nested rows in the “rows” binding. The corresponding property should be an ordered to-many relationship containing additional bound row objects.

The default value is `@"subrows"`.

## See Also

### Supporting Bindings

var rowClass: AnyClass

The class used to create a new row in the “rows” binding.

var rowTypeKeyPath: String

The key path for the row type.

var criteriaKeyPath: String

The criteria key path.

var displayValuesKeyPath: String

The display values key path.

