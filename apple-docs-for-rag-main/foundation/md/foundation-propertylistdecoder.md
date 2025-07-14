

- Foundation
-  PropertyListDecoder 

Class

# PropertyListDecoder

An object that decodes instances of data types from a property list.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class PropertyListDecoder
```

## Topics

### Decoding

init()

Creates a new, reusable property list decoder.

func decode&lt;T>(T.Type, from: Data) throws -> T

Returns a value of the specified type by decoding a property list using the default property list format.

### Customizing Decoding

func decode&lt;T>(T.Type, from: Data, format: inout PropertyListDecoder.PropertyListFormat) throws -> T

Returns a value of the specified type by decoding a property list using the supplied format.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize decoding by providing contextual information.

### Instance Methods

func decode&lt;T, C>(T.Type, from: Data, configuration: C.Type) throws -> T

func decode&lt;T>(T.Type, from: Data, configuration: T.DecodingConfiguration) throws -> T

func decode&lt;T>(T.Type, from: Data, format: inout PropertyListDecoder.PropertyListFormat, configuration: T.DecodingConfiguration) throws -> T

func decode&lt;T, C>(T.Type, from: Data, format: inout PropertyListDecoder.PropertyListFormat, configuration: C.Type) throws -> T

### Type Aliases

typealias PropertyListFormat

## Relationships

### Conforms To

- Copyable
- Sendable
- TopLevelDecoder

## See Also

### Property Lists

class PropertyListEncoder

An object that encodes instances of data types to a property list.

class PropertyListSerialization

An object that converts between a property list and one of several serialized representations.

