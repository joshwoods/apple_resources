

- TabularData
-  CSVWritingOptions 

Structure

# CSVWritingOptions

A set of CSV file-writing options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct CSVWritingOptions
```

## Topics

### Initializers

init()

Creates the default set of options for writing a CSV file.

init(includesHeader: Bool, dateFormat: String?, nilEncoding: String, trueEncoding: String, falseEncoding: String, newline: String, delimiter: Character)

Creates a set of options for writing a CSV file.

Deprecated

init(includesHeader: Bool, nilEncoding: String, trueEncoding: String, falseEncoding: String, newline: String, delimiter: Character)

Creates a set of options for writing a CSV file.

### Instance Properties

var dateFormat: String?

The format the CSV file generator uses to create date strings.

Deprecated

var dateFormatter: (Date) -> String

A closure that maps dates to their string representations.

var delimiter: Character

The character the CSV file generator uses to separate data fields in a CSV file.

var falseEncoding: String

The string the CSV file generator uses to represent false Boolean values.

var includesHeader: Bool

A Boolean value that indicates whether to write a header with the column names.

var newline: String

The string the CSV file generator uses to represent a newline sequence.

var nilEncoding: String

The string the CSV file generator uses to represent nil values.

var trueEncoding: String

The string the CSV file generator uses to represent true Boolean values.

## See Also

### Saving a Data Frame to a CSV Format

func writeCSV(to: URL, options: CSVWritingOptions) throws

Creates a CSV file with the contents of the data frame type.

func csvRepresentation(options: CSVWritingOptions) throws -> Data

Generates a CSV data instance of the data frame type.

