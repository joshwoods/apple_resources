

- TabularData
- DataFrame
-  writeCSV(to:options:) 

Instance Method

# writeCSV(to:options:)

Creates a CSV file with the contents of the data frame type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func writeCSV(
    to url: URL,
    options: CSVWritingOptions = .init()
) throws
```

## Parameters 

`url`  

A location URL in the file system where the method saves the CSV file.

`options`  

A CSVWritingOptions instance.

## See Also

### Saving a Data Frame to a CSV Format

func csvRepresentation(options: CSVWritingOptions) throws -> Data

Generates a CSV data instance of the data frame type.

struct CSVWritingOptions

A set of CSV file-writing options.

