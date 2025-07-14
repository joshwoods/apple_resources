

- Foundation
-  PropertyListEncoder 

Class

# PropertyListEncoder

An object that encodes instances of data types to a property list.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class PropertyListEncoder
```

## Mentioned in 

Encoding and Decoding Custom Types

## Topics

### Encoding

init()

Creates a new, reusable property list encoder with the default formatting settings.

func encode&lt;Value>(Value) throws -> Data

Returns a property list that represents an encoded version of the value you supply.

func encode&lt;T, C>(T, configuration: C.Type) throws -> Data

func encode&lt;T>(T, configuration: T.EncodingConfiguration) throws -> Data

### Customizing Encoding

var outputFormat: PropertyListDecoder.PropertyListFormat

A value that determines which property list format is used during encoding.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize the encoding process by providing contextual information.

## Relationships

### Conforms To

- Copyable
- Sendable
- TopLevelEncoder

## See Also

### Property Lists

class PropertyListDecoder

An object that decodes instances of data types from a property list.

class PropertyListSerialization

An object that converts between a property list and one of several serialized representations.

