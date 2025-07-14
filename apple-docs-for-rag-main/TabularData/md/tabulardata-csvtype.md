

- TabularData
-  CSVType 

Enumeration

# CSVType

Represents the value types in a CSV file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum CSVType
```

## Topics

### Operators

static func == (CSVType, CSVType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case boolean

A Boolean type.

case data

A binary data type.

case date

A date type.

case double

A double-precision floating-point type.

case float

A single-precision floating-point type.

case integer

An integer type.

case string

A string type.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a Data Frame from a CSV

init(contentsOfCSVFile: URL, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from a CSV file.

init(csvData: Data, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from CSV data.

struct CSVReadingOptions

A set of CSV file-reading options.

