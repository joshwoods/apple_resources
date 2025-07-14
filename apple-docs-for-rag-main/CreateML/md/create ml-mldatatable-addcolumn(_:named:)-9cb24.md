

- Create ML
- MLDataTable
-  addColumn(\_:named:) 

Instance Method

# addColumn(\_:named:)

Adds an untyped column to the table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
mutating func addColumn(
    _ newColumn: MLUntypedColumn,
    named: String
)
```

## Parameters 

`newColumn`  

A column to add to the data table.

`named`  

The name of the new column.

## Discussion

Use this method to add an untyped column to a data table.

Important

The number of elements in the column must equal the number of rows in the data table. Otherwise, the data table will be invalidated.

As an example, start with a data table variable.

```
let data: [String: MLDataValueConvertible] = [
    "Title": ["Alice in Wonderland", "Hamlet", "Treasure Island", "Peter Pan"],
    "Author": ["Lewis Carroll", "William Shakespeare", "Robert L. Stevenson", "J. M. Barrie"],
    "Pages": [124, 98, 280, 94],
]

var bookTable = try MLDataTable(dictionary: data)
```

Then use addColumn(_:named:) to add a column to the table.

```
let pagesColumn = MLUntypedColumn([124, 98, 280, 94])
bookTable.addColumn(pagesColumn, named: "Pages")
```

## See Also

### Adding columns

func addColumn&lt;Element>(MLDataColumn&lt;Element>, named: String)

Adds a data column to the table.

struct MLDataColumn

A column of typed values in a data table.

struct MLUntypedColumn

A column of untyped values in a data table.

