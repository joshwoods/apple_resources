

- Create ML
- MLDataTable
-  init(namedColumns:) 

Initializer

# init(namedColumns:)

Creates a data table from a dictionary of column names and untyped columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(namedColumns: [String : MLUntypedColumn]) throws
```

## Parameters 

`namedColumns`  

The dictionary of each column name and its associated untyped column data.

## Discussion

Use this initializer to create a data table from untyped columns.

For example, to create a data table as shown above, first create your untyped columns.

```
let pages = MLUntypedColumn([124, 98, 280, 94])
let genre = MLUntypedColumn(["Fantasy", "Drama", "Adventure", "Fantasy"])
let title = MLUntypedColumn(["Alice in Wonderland", "Hamlet", "Treasure Island", "Peter Pan"])
let author = MLUntypedColumn(["Lewis Carroll", "William Shakespeare", "Robert L. Stevenson", "J. M. Barrie"])
```

Then, use init(namedColumns:) to create a data table from the columns paired with their names.

```
let bookTable = try MLDataTable(namedColumns: ["Title": title,
                                               "Author": author,
                                               "Pages": pages,
                                               "Genre": genre])
```

## See Also

### Creating a data table

Creating a Model from Tabular Data

Train a machine learning model by using Core ML to import and manage tabular data.

init(contentsOf: URL, options: MLDataTable.ParsingOptions) throws

Creates a data table from an imported JSON or CSV file.

init(dictionary: [String : any MLDataValueConvertible]) throws

Creates a data table from a dictionary of column names and data values.

init()

Creates an empty table containing no rows or columns.

