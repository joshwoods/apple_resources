

- XCTest
- XCTSourceCodeContext
-  callStack 

Instance Property

# callStack

An array of source code frames that describes the call stack when a test issue occurs.

``` source
var callStack: [XCTSourceCodeFrame] { get }
```

## See Also

### Context Information

var location: XCTSourceCodeLocation?

A representation of a location in source code where a test issue occurred.

