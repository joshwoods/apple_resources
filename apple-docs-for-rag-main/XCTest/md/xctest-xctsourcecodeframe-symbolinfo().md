

- XCTest
- XCTSourceCodeFrame
-  symbolInfo() 

Instance Method

# symbolInfo()

Attempts to get symbol information for the address.

``` source
func symbolInfo() throws -> XCTSourceCodeSymbolInfo
```

## Return Value

Symbol information for the address.

## Discussion

This method can fail if required symbol data is not available. The system makes only one attempt to retrieve the symbol information. If that attempt fails, the system stores the error and returns it for future requests.

## See Also

### Frame Information

var address: UInt64

An address that represents a specific frame in a call stack.

var symbolInfo: XCTSourceCodeSymbolInfo?

Symbolication information for the referenced frame.

var symbolicationError: (any Error)?

An optional error that describes a failed symbolication attempt.

