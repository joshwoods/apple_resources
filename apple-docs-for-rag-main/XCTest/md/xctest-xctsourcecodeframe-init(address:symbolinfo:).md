

- XCTest
- XCTSourceCodeFrame
-  init(address:symbolInfo:) 

Initializer

# init(address:symbolInfo:)

Initializes an instance with a frame address and symbol information.

``` source
init(
    address: UInt64,
    symbolInfo: XCTSourceCodeSymbolInfo?
)
```

## Parameters 

`address`  

An address that represents a specific frame in a call stack.

`symbolInfo`  

Symbolication information for the referenced frame.

## See Also

### Initializers

convenience init(address: UInt64)

Initializes an instance with a frame address.

