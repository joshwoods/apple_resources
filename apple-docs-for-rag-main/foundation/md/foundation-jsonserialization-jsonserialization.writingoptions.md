

- Foundation
- JSONSerialization
-  JSONSerialization.WritingOptions 

Structure

# JSONSerialization.WritingOptions

Options for writing JSON data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct WritingOptions
```

## Topics

### Creating a Writing Options Instance

init(rawValue: UInt)

### Formatting JSON

static var fragmentsAllowed: JSONSerialization.WritingOptions

Specifies that the parser should allow top-level objects that aren’t arrays or dictionaries.

static var prettyPrinted: JSONSerialization.WritingOptions

Specifies that the output uses white space and indentation to make the resulting data more readable.

static var sortedKeys: JSONSerialization.WritingOptions

Specifies that the output sorts keys in lexicographic order.

static var withoutEscapingSlashes: JSONSerialization.WritingOptions

Specifies that the output doesn’t prefix slash characters with escape characters.

static var fragmentsAllowed: JSONSerialization.WritingOptions

Specifies that the parser should allow top-level objects that aren’t arrays or dictionaries.

static var prettyPrinted: JSONSerialization.WritingOptions

Specifies that the output uses white space and indentation to make the resulting data more readable.

static var sortedKeys: JSONSerialization.WritingOptions

Specifies that the output sorts keys in lexicographic order.

static var withoutEscapingSlashes: JSONSerialization.WritingOptions

Specifies that the output doesn’t prefix slash characters with escape characters.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating JSON Data

class func data(withJSONObject: Any, options: JSONSerialization.WritingOptions) throws -> Data

Returns JSON data from a Foundation object.

class func writeJSONObject(Any, to: OutputStream, options: JSONSerialization.WritingOptions, error: NSErrorPointer) -> Int

Writes a given JSON object to a stream.

class func isValidJSONObject(Any) -> Bool

Returns a Boolean value that indicates whether the serializer can convert a given object to JSON data.

