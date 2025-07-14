

- XCTest
-  XCTSourceCodeSymbolInfo 

Class

# XCTSourceCodeSymbolInfo

An object that contains symbolication information for a specified frame in a call stack.

``` source
class XCTSourceCodeSymbolInfo
```

## Topics

### Initializers

init(imageName: String, symbolName: String, location: XCTSourceCodeLocation?)

Initializes an instance with a binary image name, source code location, and symbol name.

### Symbol Information

var imageName: String

The name of the binary image that contains the symbolicated code.

var location: XCTSourceCodeLocation?

A representation of a location in source code where a test issue occurred.

var symbolName: String

A string that represents a human-readable symbol in source code.

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

class XCTSourceCodeFrame

An object that represents a single frame in a call stack that supports retrieval of symbol information for the address.

class XCTSourceCodeLocation

An object that contains a file URL and line number that represents a distinct location in source code.

