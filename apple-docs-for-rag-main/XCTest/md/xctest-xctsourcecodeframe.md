

- XCTest
-  XCTSourceCodeFrame 

Class

# XCTSourceCodeFrame

An object that represents a single frame in a call stack that supports retrieval of symbol information for the address.

``` source
class XCTSourceCodeFrame
```

## Topics

### Initializers

init(address: UInt64, symbolInfo: XCTSourceCodeSymbolInfo?)

Initializes an instance with a frame address and symbol information.

convenience init(address: UInt64)

Initializes an instance with a frame address.

### Frame Information

var address: UInt64

An address that represents a specific frame in a call stack.

var symbolInfo: XCTSourceCodeSymbolInfo?

Symbolication information for the referenced frame.

var symbolicationError: (any Error)?

An optional error that describes a failed symbolication attempt.

func symbolInfo() throws -> XCTSourceCodeSymbolInfo

Attempts to get symbol information for the address.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Test Failures

struct XCTIssue

An object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTIssueReference

An object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTMutableIssue

A mutable object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTSourceCodeContext

An object that contains call stack and source code location details to provide context for a point of execution in a test.

class XCTSourceCodeLocation

An object that contains a file URL and line number that represents a distinct location in source code.

class XCTSourceCodeSymbolInfo

An object that contains symbolication information for a specified frame in a call stack.

