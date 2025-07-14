

- TabularData
- DataFrameProtocol
-  csvRepresentation(options:) 

Instance Method

# csvRepresentation(options:)

Generates a CSV data instance of the data frame type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func csvRepresentation(options: CSVWritingOptions = .init()) throws -> Data
```

## Parameters 

`options`  

A CSVWritingOptions instance.

## See Also

### Saving a Data Frame Type to a CSV Format

func writeCSV(to: URL, options: CSVWritingOptions) throws

Creates a CSV file with the contents of the data frame type.

