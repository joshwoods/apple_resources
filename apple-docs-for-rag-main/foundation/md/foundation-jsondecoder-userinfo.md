

- Foundation
- JSONDecoder
-  userInfo 

Instance Property

# userInfo

A dictionary you use to customize the decoding process by providing contextual information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
var userInfo: [CodingUserInfoKey : any Sendable] { get set }
```

## See Also

### Customizing Decoding

var keyDecodingStrategy: JSONDecoder.KeyDecodingStrategy

A value that determines how to decode a type’s coding keys from JSON keys.

enum KeyDecodingStrategy

The values that determine how to decode a type’s coding keys from JSON keys.

var allowsJSON5: Bool

Specifies that decoding supports the JSON5 syntax.

var assumesTopLevelDictionary: Bool

Specifies that decoding assumes the top level of the JSON data is a dictionary, even if it doesn’t begin and end with braces.

