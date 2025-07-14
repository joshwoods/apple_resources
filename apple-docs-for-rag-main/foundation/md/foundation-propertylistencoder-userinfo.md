

- Foundation
- PropertyListEncoder
-  userInfo 

Instance Property

# userInfo

A dictionary you use to customize the encoding process by providing contextual information.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@preconcurrency
var userInfo: [CodingUserInfoKey : any Sendable] { get set }
```

## See Also

### Customizing Encoding

var outputFormat: PropertyListDecoder.PropertyListFormat

A value that determines which property list format is used during encoding.

