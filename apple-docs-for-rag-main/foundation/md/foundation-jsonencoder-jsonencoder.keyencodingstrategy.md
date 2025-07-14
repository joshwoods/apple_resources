

- Foundation
- JSONEncoder
-  JSONEncoder.KeyEncodingStrategy 

Enumeration

# JSONEncoder.KeyEncodingStrategy

The values that determine how to encode a type’s coding keys as JSON keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum KeyEncodingStrategy
```

## Overview

Note

Key encoding strategies other than JSONEncoder.KeyEncodingStrategy.useDefaultKeys may have a noticeable performance cost because those strategies may inspect and transform each key.

## Topics

### Built-in Encoding

case convertToSnakeCase

A key encoding strategy that converts camel-case keys to snake-case keys.

case useDefaultKeys

A key encoding strategy that doesn’t change key names during encoding.

### Custom Encoding

case custom(([any CodingKey]) -> any CodingKey)

A key encoding strategy defined by the closure you supply.

## Relationships

### Conforms To

- Sendable

## See Also

### Customizing Encoding

var outputFormatting: JSONEncoder.OutputFormatting

A value that determines the readability, size, and element order of the encoded JSON object.

struct OutputFormatting

The output formatting options that determine the readability, size, and element order of an encoded JSON object.

var keyEncodingStrategy: JSONEncoder.KeyEncodingStrategy

A value that determines how to encode a type’s coding keys as JSON keys.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize the encoding process by providing contextual information.

