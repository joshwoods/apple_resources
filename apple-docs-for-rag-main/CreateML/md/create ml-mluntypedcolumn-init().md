

- Create ML
- MLUntypedColumn
-  init() 

Initializer

# init()

Creates an empty, invalid column used to remove an existing column from a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init()
```

## Return Value

An empty, invalid column.

## Discussion

Use this initializer to create an empty column that, when assigned to the name of an existing column within a data table, will remove that column from the table.

For example, to remove a column from a data table, first start with a variable data table.

```
let data: [String: MLDataValueConvertible] = [
    "Day": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
    "Temperature": [91.3, 85.8, 79.5, 83.4, 72.2]
]

var table = try MLDataTable(dictionary: data)

print(table)
/* Prints...
 Columns:
 Day    string
 Temperature    float
 Rows: 5
 Data:
 +----------------+----------------+
 | Day            | Temperature    |
 +----------------+----------------+
 | Monday         | 91.3           |
 | Tuesday        | 85.8           |
 | Wednesday      | 79.5           |
 | Thursday       | 83.4           |
 | Friday         | 72.2           |
 +----------------+----------------+
 [5 rows x 2 columns]
 */
```

Then use init() to create an empty column.

```
let emptyColumn = MLUntypedColumn()
```

Finally, use subscript(_:) to remove the existing column from the data table by setting the empty column to the name of that existing column.

```
// Remove the "Temperature" column from the data table
table["Temperature"] = emptyColumn

print(table)
/* Prints...
 Columns:
 Day    string
 Rows: 5
 Data:
 +----------------+
 | Day            |
 +----------------+
 | Monday         |
 | Tuesday        |
 | Wednesday      |
 | Thursday       |
 | Friday         |
 +----------------+
 [5 rows x 1 columns]
 */
```

## See Also

### Creating an untyped column

init&lt;T>(repeating: T, count: Int)

Creates a new column with a repeating value.

init(repeating: MLDataValue, count: Int)

Creates a new column with a repeating value.

init(Range&lt;Int>)

Creates a new column of integers from a given range.

init(ClosedRange&lt;Int>)

Creates a new column of integers from a given closed range.

init&lt;S>(S)

Creates a new column from a given sequence of elements that can be converted to machine learning data values.

init&lt;S>(S)

Creates a new column from a given sequence of machine learning data values.

