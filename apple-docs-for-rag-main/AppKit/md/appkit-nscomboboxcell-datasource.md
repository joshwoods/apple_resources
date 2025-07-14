

- AppKit
- NSComboBoxCell
-  dataSource 

Instance Property

# dataSource

The object that provides the data displayed in the combo box’s pop-up list.

macOS

``` source
@MainActor
unowned(unsafe) var dataSource: (any NSComboBoxCellDataSource)? { get set }
```

## Discussion

The value of this property should be an object that implements the appropriate methods of the NSComboBoxCellDataSource informal protocol. Note that setting this property doesn’t automatically set usesDataSource to false and in fact logs a warning if usesDataSource is false. If you set this property to an object that doesn’t respond to either numberOfItemsInComboBoxCell: or comboBoxCell:objectValueForItemAtIndex:, a warning is logged if usesDataSource is false. See the class description and the NSComboBoxCellDataSource informal protocol specification for more information on combo box cell data source objects.

## See Also

### Accessing a Data Source

var usesDataSource: Bool

A Boolean value that indicates if the combo box uses an external data source to populate its pop-up list.

