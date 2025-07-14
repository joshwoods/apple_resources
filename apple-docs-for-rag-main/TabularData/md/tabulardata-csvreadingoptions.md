

- TabularData
-  CSVReadingOptions 

Structure

# CSVReadingOptions

A set of CSV file-reading options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct CSVReadingOptions
```

## Topics

### Initializers

init(hasHeaderRow: Bool, nilEncodings: Set&lt;String>, trueEncodings: Set&lt;String>, falseEncodings: Set&lt;String>, floatingPointType: CSVType, ignoresEmptyLines: Bool, usesQuoting: Bool, usesEscaping: Bool, delimiter: Character, escapeCharacter: Character)

Creates a set of options for reading a CSV file.

### Instance Properties

var dateParsers: [(String) -> Date?]

An array of closures that parse a date from a string.

var delimiter: Character

The character that separates data fields in a CSV file, typically a comma.

var escapeCharacter: Character

The character that precedes other characters, such as quotation marks, so that the parser interprets them as literal characters instead of special ones.

var falseEncodings: Set&lt;String>

The set of strings that stores acceptable spellings for false Boolean values.

var floatingPointType: CSVType

The type to use for floating-point numeric values.

var hasHeaderRow: Bool

A Boolean value that indicates whether the CSV file has a header row.

var ignoresEmptyLines: Bool

A Boolean value that indicates whether to ignore empty lines.

var nilEncodings: Set&lt;String>

The set of strings that stores acceptable spellings for empty values.

var trueEncodings: Set&lt;String>

The set of strings that stores acceptable spellings for true Boolean values.

var usesEscaping: Bool

A Boolean value that indicates whether to enable escaping.

var usesQuoting: Bool

A Boolean value that indicates whether to enable quoting.

### Instance Methods

func addDateParseStrategy&lt;T>(T)

Adds a date parsing strategy.

## See Also

### Creating a Data Frame from a CSV

init(contentsOfCSVFile: URL, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from a CSV file.

init(csvData: Data, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from CSV data.

enum CSVType

Represents the value types in a CSV file.

