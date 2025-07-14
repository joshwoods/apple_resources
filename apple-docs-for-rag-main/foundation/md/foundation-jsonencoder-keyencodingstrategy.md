

- Foundation
- JSONEncoder
-  keyEncodingStrategy 

Instance Property

# keyEncodingStrategy

A value that determines how to encode a type’s coding keys as JSON keys.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var keyEncodingStrategy: JSONEncoder.KeyEncodingStrategy { get set }
```

## See Also

### Customizing Encoding

var outputFormatting: JSONEncoder.OutputFormatting

A value that determines the readability, size, and element order of the encoded JSON object.

struct OutputFormatting

The output formatting options that determine the readability, size, and element order of an encoded JSON object.

enum KeyEncodingStrategy

The values that determine how to encode a type’s coding keys as JSON keys.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize the encoding process by providing contextual information.

