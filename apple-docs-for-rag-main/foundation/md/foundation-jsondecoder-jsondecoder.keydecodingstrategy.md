

- Foundation
- JSONDecoder
-  JSONDecoder.KeyDecodingStrategy 

Enumeration

# JSONDecoder.KeyDecodingStrategy

The values that determine how to decode a type’s coding keys from JSON keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum KeyDecodingStrategy
```

## Overview

Note

Key decoding strategies other than JSONDecoder.KeyDecodingStrategy.useDefaultKeys may have a noticeable performance cost because those strategies may inspect and transform each key.

## Topics

### Built-in Decoding

case convertFromSnakeCase

A key decoding strategy that converts snake-case keys to camel-case keys.

case useDefaultKeys

A key decoding strategy that doesn’t change key names during decoding.

### Custom Decoding

case custom(([any CodingKey]) -> any CodingKey)

A key decoding strategy defined by the closure you supply.

## Relationships

### Conforms To

- Sendable

## See Also

### Customizing Decoding

var keyDecodingStrategy: JSONDecoder.KeyDecodingStrategy

A value that determines how to decode a type’s coding keys from JSON keys.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize the decoding process by providing contextual information.

var allowsJSON5: Bool

Specifies that decoding supports the JSON5 syntax.

var assumesTopLevelDictionary: Bool

Specifies that decoding assumes the top level of the JSON data is a dictionary, even if it doesn’t begin and end with braces.

