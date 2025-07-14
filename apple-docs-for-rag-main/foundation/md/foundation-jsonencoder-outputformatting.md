

- Foundation
- JSONEncoder
-  outputFormatting 

Instance Property

# outputFormatting

A value that determines the readability, size, and element order of the encoded JSON object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outputFormatting: JSONEncoder.OutputFormatting { get set }
```

## See Also

### Customizing Encoding

struct OutputFormatting

The output formatting options that determine the readability, size, and element order of an encoded JSON object.

var keyEncodingStrategy: JSONEncoder.KeyEncodingStrategy

A value that determines how to encode a type’s coding keys as JSON keys.

enum KeyEncodingStrategy

The values that determine how to encode a type’s coding keys as JSON keys.

var userInfo: [CodingUserInfoKey : any Sendable]

A dictionary you use to customize the encoding process by providing contextual information.

