

- TabularData
-  JSONReadingOptions 

Structure

# JSONReadingOptions

A set of JSON file-reading options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct JSONReadingOptions
```

## Topics

### Initializers

init()

Creates a set of options for reading a JSON file.

### Instance Properties

var dateParsers: [(String) -> Date?]

An array of closures that parse a date from a string.

### Instance Methods

func addDateParseStrategy&lt;T>(T)

Adds a date parsing strategy.

## See Also

### Creating a Data Frame from a JSON File

init(contentsOfJSONFile: URL, columns: [String]?, types: [String : JSONType], options: JSONReadingOptions) throws

Creates a data frame by reading a JSON file.

init(jsonData: Data, columns: [String]?, types: [String : JSONType], options: JSONReadingOptions) throws

Creates a data frame by converting JSON data.

enum JSONType

Represents the value types in a JSON file.

