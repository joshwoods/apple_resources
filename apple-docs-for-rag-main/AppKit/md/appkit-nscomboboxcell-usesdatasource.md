

- AppKit
- NSComboBoxCell
-  usesDataSource 

Instance Property

# usesDataSource

A Boolean value that indicates if the combo box uses an external data source to populate its pop-up list.

macOS

``` source
@MainActor
var usesDataSource: Bool { get set }
```

## Discussion

When the value of this property is true, the combo box uses an external data source to populate its pop-up list; when it is false, the combo box uses an internal item list.

## See Also

### Accessing a Data Source

var dataSource: (any NSComboBoxCellDataSource)?

The object that provides the data displayed in the combo box’s pop-up list.

