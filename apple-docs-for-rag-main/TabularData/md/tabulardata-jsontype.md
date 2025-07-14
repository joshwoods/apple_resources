

- TabularData
-  JSONType 

Enumeration

# JSONType

Represents the value types in a JSON file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum JSONType
```

## Topics

### Operators

static func == (JSONType, JSONType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case array

An array type.

case boolean

A Boolean type.

case date

A date type.

case double

A double-precision floating-point type.

case integer

An integer type.

case object

An object type.

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

### Creating a Data Frame from a JSON File

init(contentsOfJSONFile: URL, columns: [String]?, types: [String : JSONType], options: JSONReadingOptions) throws

Creates a data frame by reading a JSON file.

init(jsonData: Data, columns: [String]?, types: [String : JSONType], options: JSONReadingOptions) throws

Creates a data frame by converting JSON data.

struct JSONReadingOptions

A set of JSON file-reading options.

