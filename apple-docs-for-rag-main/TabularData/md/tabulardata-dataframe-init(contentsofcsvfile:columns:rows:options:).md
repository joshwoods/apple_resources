

- TabularData
- DataFrame
-  init(contentsOfCSVFile:columns:rows:options:) 

Initializer

# init(contentsOfCSVFile:columns:rows:options:)

Creates a data frame from a CSV file.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
init(
    contentsOfCSVFile url: URL,
    columns: repeat ColumnID,
    rows: Range? = nil,
    options: CSVReadingOptions = .init()
) throws
```

## Parameters 

`url`  

A URL for a CSV file.

`columns`  

The column identifiers.

`rows`  

A range of indices; Set to `nil` to use every row in the CSV file.

`options`  

The options that tell the data frame how to read the CSV file.

