

- TabularData
- DataFrame
-  init(contentsOfCSVFile:columns:rows:types:options:) 

Initializer

# init(contentsOfCSVFile:columns:rows:types:options:)

Creates a data frame from a CSV file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    contentsOfCSVFile url: URL,
    columns: [String]? = nil,
    rows: Range? = nil,
    types: [String : CSVType] = [:],
    options: CSVReadingOptions = .init()
) throws
```

## Parameters 

`url`  

A URL for a CSV file.

`columns`  

An array of column names; Set to `nil` to use every column in the CSV file.

`rows`  

A range of indices; Set to `nil` to use every row in the CSV file.

`types`  

A dictionary of column names and their CSV types. The data frame infers the types for column names that aren’t in the dictionary.

`options`  

The options that tell the data frame how to read the CSV file.

## Discussion

Throws

A `CSVReadingError` instance.

## See Also

### Creating a Data Frame from a CSV

init(csvData: Data, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from CSV data.

enum CSVType

Represents the value types in a CSV file.

struct CSVReadingOptions

A set of CSV file-reading options.

