

- AppKit
- NSComboBox
-  usesDataSource 

Instance Property

# usesDataSource

A Boolean value indicating whether the combo box retrieves its items from a data source object.

macOS

``` source
@MainActor
var usesDataSource: Bool { get set }
```

## Discussion

When the value of this property is true, the combo box retrieves its items from the object in the dataSource property. When the value is false, the combo box manages an internal list of items, which it gets from the ones specified at design time and the ones you add programmatically.

## See Also

### Setting a Data Source

var dataSource: (any NSComboBoxDataSource)?

The object that provides the item data for the combo box.

