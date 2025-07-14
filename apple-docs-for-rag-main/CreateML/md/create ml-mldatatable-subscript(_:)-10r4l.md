

- Create ML
- MLDataTable
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Creates a subset of the table by masking the rows with the given untyped column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(mask: MLUntypedColumn) -> MLDataTable { get }
```

## Parameters 

`mask`  

An untyped column indicating whether rows should be removed (a default value) or included (any nondefault value) in the derived table.

## Return Value

A new data table.

## Overview

Use this untyped column–based subscript to create a new table by masking a subset of the table rows. The derived table will not include rows where `mask` contains a default value for its underlying type, such as:

- `0` in untyped `Int` columns

- `0.0` in untyped `Double` columns

- An empty string in untyped `String` columns

The derived data table includes rows where the masking column has any other (nondefault) value.

For example, to filter the values in a data table as shown above, begin by creating a table with the original data.

```
let data: [String: MLDataValueConvertible] = [
    "Title": ["Alice in Wonderland", "Hamlet", "Dracula", "Peter Pan", "The Great Gatsby"],
    "Genre": ["Fantasy", "Drama", "Adventure", "Fantasy", "Drama"],
    "Pages": [124, 98, 0, 94, 0]
]

guard let table = try? MLDataTable(dictionary: data) else {
    fatalError("Invalid dictionary data")
}
```

After you create the table, use the `String`-based subscript(_:) to extract a column.

```
// Create a new untyped column "pagesColumn" copied from the table’s "Pages" column
let pagesColumn = table["Pages"]
```

Use `subscript(mask: MLUntypedColumn)` with an untyped column–row mask to create a filtered table. The subscript uses the untyped values to determine whether to keep a row.

In this example, the untyped column `pagesColumn` has an underlying type of `Int`. The subscript removes any row with a value of `0` (the default value for `Int`) and keeps all other rows.

```
// Filter the table using pagesColumn.
// Each row with a value of 0 is removed.
let validPageCountTable = table[pagesColumn]
```

## See Also

### Masking Rows

subscript(MLDataColumn&lt;Bool>) -> MLDataTable

Creates a subset of the table by masking the rows with the given column of Booleans.

