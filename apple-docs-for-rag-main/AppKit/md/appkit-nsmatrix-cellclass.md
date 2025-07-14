

- AppKit
- NSMatrix
-  cellClass 

Instance Property

# cellClass

The subclass of NSCell that the matrix uses when creating new (empty) cells.

macOS

``` source
@MainActor
var cellClass: AnyClass { get set }
```

## Discussion

The value of this property should be the id of a subclass of NSCell, which can be obtained by sending the `class` message to either the NSCell subclass object or to an instance of that subclass. The default cell class is that set with the class method `setCellClass(_:)`, or NSActionCell if no other default cell class has been specified.

You need to use this property only with matrices initialized with init(frame:), because the other initializers allow you to specify an instance-specific cell class or cell prototype.

## See Also

### Related Documentation

func insertColumn(Int)

Inserts a new column of cells at the specified location. .

func addRow()

Adds a new row of cells below the last row.

func addColumn()

Adds a new column of cells to the right of the last column.

func insertRow(Int)

Inserts a new row of cells before the specified row.

func makeCell(atRow: Int, column: Int) -> NSCell

Creates a new cell at the location specified by the given row and column in the receiver.

### Managing the Cell Class

var prototype: NSCell?

The prototype cell that’s copied whenever the matrix creates a new cell.

