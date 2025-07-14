

- XCTest
- XCTSourceCodeFrame
-  symbolInfo 

Instance Property

# symbolInfo

Symbolication information for the referenced frame.

``` source
var symbolInfo: XCTSourceCodeSymbolInfo? { get }
```

## See Also

### Frame Information

var address: UInt64

An address that represents a specific frame in a call stack.

var symbolicationError: (any Error)?

An optional error that describes a failed symbolication attempt.

func symbolInfo() throws -> XCTSourceCodeSymbolInfo

Attempts to get symbol information for the address.

