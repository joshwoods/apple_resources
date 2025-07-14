

- TabularData
- DataFrame
-  init(csvData:columns:rows:options:) 

Initializer

# init(csvData:columns:rows:options:)

Creates a data frame from CSV data.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
init(
    csvData data: Data,
    columns: repeat ColumnID,
    rows: Range? = nil,
    options: CSVReadingOptions = .init()
) throws
```

## Parameters 

`data`  

The contents of a CSV file.

`columns`  

The column identifiers.

`rows`  

A range of indices; Set to `nil` to use every row in the CSV file.

`options`  

The options that tell the data frame how to read the CSV data.

