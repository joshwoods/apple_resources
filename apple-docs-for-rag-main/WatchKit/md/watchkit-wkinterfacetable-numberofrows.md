

- WatchKit
- WKInterfaceTable
-  numberOfRows 

Instance Property

# numberOfRows

The number of row controllers available for you to retrieve.

watchOS 2.0+

``` source
var numberOfRows: Int { get }
```

## Discussion

The value of this property is `0` until you call the setRowTypes(_:) or setNumberOfRows(_:withRowType:) method. After calling one of those methods, this property contains the number of row controllers that were created.

## See Also

### Getting the Row Controllers

func rowController(at: Int) -> Any?

Returns the row controller for the row at the specified index in the table.

