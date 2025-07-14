

- Foundation
- JSONEncoder
-  JSONEncoder.OutputFormatting 

Structure

# JSONEncoder.OutputFormatting

The output formatting options that determine the readability, size, and element order of an encoded JSON object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct OutputFormatting
```

## Topics

### Formatting Output

static let prettyPrinted: JSONEncoder.OutputFormatting

The output formatting option that uses ample white space and indentation to make output easy to read.

static let sortedKeys: JSONEncoder.OutputFormatting

The output formatting option that sorts keys in lexicographic order.

static let withoutEscapingSlashes: JSONEncoder.OutputFormatting

The output formatting option specifies that the output doesn’t prefix slash characters with escape characters.

### Creating Options

init(rawValue: UInt)

Creates an OutputFormatting value with the given raw value.

let rawValue: UInt

The format’s default value.

init()

Creates a new, reusable JSON encoder with the default formatting settings and encoding strategies.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Customizing Encoding

var outputFormatting: JSONEncoder.OutputFormatting

A value that determines the readability, size, and element order of the encoded JSON object.

var keyEncodingStrategy: JSONEncoder.KeyEncodingStrategy

A value that determines how to encode a type’s coding keys as JSON keys.

enum KeyEncodingStrategy

The values that determine how to encode a type’s coding keys as JSON keys.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize the encoding process by providing contextual information.

