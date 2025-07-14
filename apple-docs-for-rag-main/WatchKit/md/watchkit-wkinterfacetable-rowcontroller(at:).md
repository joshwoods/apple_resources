

- WatchKit
- WKInterfaceTable
-  rowController(at:) 

Instance Method

# rowController(at:)

Returns the row controller for the row at the specified index in the table.

watchOS 2.0+

``` source
func rowController(at index: Int) -> Any?
```

## Parameters 

`index`  

The zero-based index of the row. This parameter must be between zero and the total number of rows specified in the numberOfRows property.

## Return Value

The row controller object, or `nil` if there are no row controllers yet or `index` is out of bounds.

## Discussion

Call the setRowTypes(_:) or setNumberOfRows(_:withRowType:) method before using this method to retrieve any row controllers. After you call one of those methods, the table creates row controllers for each row type and stores them internally in an array. Use this method to retrieve those row controllers.

## See Also

### Getting the Row Controllers

var numberOfRows: Int

The number of row controllers available for you to retrieve.

