

- Create ML
- MLDataTable
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the table by masking the rows with the given column of Booleans.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(mask: MLDataColumn) -> MLDataTable { get }
```

## Parameters 

`mask`  

A Boolean column indicating whether rows should be kept (`true`) or removed (`false`) in the derived table.

## Return Value

A new data table.

## Overview

Use this Boolean column–based subscript to create a new table by masking a subset of the table rows.

For example, to filter the values in a data table as shown above, begin by creating a table with the original data.

```
let data: [String: MLDataValueConvertible] = [
    "Title": ["Alice in Wonderland", "Hamlet", "Treasure Island", "Peter Pan"],
    "Genre": ["Fantasy", "Drama", "Adventure", "Fantasy"]
]

let table = try? MLDataTable(dictionary: data) else {
    fatalError("Invalid dictionary data")
}
```

After you create the table, use column arithmetic operators or the map(_:) method to build a row mask. The subscript uses the Boolean values in the row mask to determine whether to keep a row.

```
// Retrieve the "Genre" column from the table.
guard let genreColumn = table["Genre", String.self] else {
    fatalError("Missing or invalid 'genre' column in table.")
}

// Create a new column of Booleans by comparing all of the values
// in `Genre` with `Fantasy` using the
// `!=(MLDataColumn, String) -> MLDataColumn` operator.
let noFantasyMask = genreColumn != "Fantasy"
```

Use `subscript(mask: MLDataColumn)` with the Boolean column–row mask to create a filtered table.

```
let noFantasyTable = table[noFantasyMask]
```

## See Also

### Masking Rows

subscript(MLUntypedColumn) -> MLDataTable

Creates a subset of the table by masking the rows with the given untyped column.

