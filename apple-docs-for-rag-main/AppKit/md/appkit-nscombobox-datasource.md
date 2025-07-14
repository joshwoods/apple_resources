

- AppKit
- NSComboBox
-  dataSource 

Instance Property

# dataSource

The object that provides the item data for the combo box.

macOS

``` source
@MainActor
unowned(unsafe) var dataSource: (any NSComboBoxDataSource)? { get set }
```

## Discussion

Assigning an object to this property does not automatically set the usesDataSource property to true. If the usesDataSource property is false, accessing this property logs a warning. The default value of this property is `nil`.

For information about how to implement a combo box data source, see `NSComboBoxDataSource`.

## See Also

### Setting a Data Source

var usesDataSource: Bool

A Boolean value indicating whether the combo box retrieves its items from a data source object.

