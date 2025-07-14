

- XCTest
- XCTSourceCodeFrame
-  address 

Instance Property

# address

An address that represents a specific frame in a call stack.

``` source
var address: UInt64 { get }
```

## See Also

### Frame Information

var symbolInfo: XCTSourceCodeSymbolInfo?

Symbolication information for the referenced frame.

var symbolicationError: (any Error)?

An optional error that describes a failed symbolication attempt.

func symbolInfo() throws -> XCTSourceCodeSymbolInfo

Attempts to get symbol information for the address.

