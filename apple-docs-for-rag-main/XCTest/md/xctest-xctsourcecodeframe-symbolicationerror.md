

- XCTest
- XCTSourceCodeFrame
-  symbolicationError 

Instance Property

# symbolicationError

An optional error that describes a failed symbolication attempt.

``` source
var symbolicationError: (any Error)? { get }
```

## Discussion

The system doesn’t serialize this error when it encodes the frames.

## See Also

### Frame Information

var address: UInt64

An address that represents a specific frame in a call stack.

var symbolInfo: XCTSourceCodeSymbolInfo?

Symbolication information for the referenced frame.

func symbolInfo() throws -> XCTSourceCodeSymbolInfo

Attempts to get symbol information for the address.

