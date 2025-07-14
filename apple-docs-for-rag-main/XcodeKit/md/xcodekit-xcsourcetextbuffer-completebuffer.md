

- XcodeKit
- XCSourceTextBuffer
-  completeBuffer 

Instance Property

# completeBuffer

The complete buffer’s string representation.

macOS 10.12+

``` source
var completeBuffer: String { get set }
```

## Discussion

Changes to the `lines` property are immediately reflected in this property, and vice versa.

## See Also

### Accessing Source Text

var contentUTI: String

The Uniform Type Identifier (UTI) of the content in the buffer.

