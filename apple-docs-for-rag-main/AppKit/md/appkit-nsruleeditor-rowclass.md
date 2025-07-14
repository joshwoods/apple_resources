

- AppKit
- NSRuleEditor
-  rowClass 

Instance Property

# rowClass

The class used to create a new row in the “rows” binding.

macOS

``` source
@MainActor
var rowClass: AnyClass { get set }
```

## Discussion

The default is `NSMutableDictionary`.

## See Also

### Supporting Bindings

var rowTypeKeyPath: String

The key path for the row type.

var subrowsKeyPath: String

The key path for the subrows.

var criteriaKeyPath: String

The criteria key path.

var displayValuesKeyPath: String

The display values key path.

