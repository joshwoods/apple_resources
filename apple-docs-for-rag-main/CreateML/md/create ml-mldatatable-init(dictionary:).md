

- Create ML
- MLDataTable
-  init(dictionary:) 

Initializer

# init(dictionary:)

Creates a data table from a dictionary of column names and data values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(dictionary: [String : any MLDataValueConvertible]) throws
```

## Parameters 

`dictionary`  

The dictionary of each column name and its associated data values.

## Discussion

Use this initializer to create a data table from an in-memory Dictionary.

For example, to create a data table as shown above, first create a dictionary.

```
let data: [String: MLDataValueConvertible] = [
    "Title": ["Alice in Wonderland", "Hamlet", "Treasure Island", "Peter Pan"],
    "Author": ["Lewis Carroll", "William Shakespeare", "Robert L. Stevenson", "J. M. Barrie"],
    "Pages": [124, 98, 280, 94],
    "Genre": ["Fantasy", "Drama", "Adventure", "Fantasy"]
]
```

Then, use init(dictionary:) to create a data table from the dictionary.

```
let bookTable = try MLDataTable(dictionary: data)
```

The keys of the dictionary become the column names, and the value of each key becomes the element(s) of the corresponding column in the data table.

## See Also

### Creating a data table

Creating a Model from Tabular Data

Train a machine learning model by using Core ML to import and manage tabular data.

init(contentsOf: URL, options: MLDataTable.ParsingOptions) throws

Creates a data table from an imported JSON or CSV file.

init(namedColumns: [String : MLUntypedColumn]) throws

Creates a data table from a dictionary of column names and untyped columns.

init()

Creates an empty table containing no rows or columns.

