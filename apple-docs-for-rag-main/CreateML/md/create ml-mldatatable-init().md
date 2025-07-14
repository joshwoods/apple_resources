

- Create ML
- MLDataTable
-  init() 

Initializer

# init()

Creates an empty table containing no rows or columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init()
```

## Discussion

Use this initializer to create an empty data table. Then, you add data columns with addColumn(_:named:), untyped columns with addColumn(_:named:), or another table with append(contentsOf:).

## See Also

### Creating a data table

Creating a Model from Tabular Data

Train a machine learning model by using Core ML to import and manage tabular data.

init(contentsOf: URL, options: MLDataTable.ParsingOptions) throws

Creates a data table from an imported JSON or CSV file.

init(dictionary: [String : any MLDataValueConvertible]) throws

Creates a data table from a dictionary of column names and data values.

init(namedColumns: [String : MLUntypedColumn]) throws

Creates a data table from a dictionary of column names and untyped columns.

