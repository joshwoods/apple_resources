

- XCTest
-  XCTSourceCodeContext 

Class

# XCTSourceCodeContext

An object that contains call stack and source code location details to provide context for a point of execution in a test.

``` source
class XCTSourceCodeContext
```

## Topics

### Initializers

init(callStack: [XCTSourceCodeFrame], location: XCTSourceCodeLocation?)

Initializes a new instance with a provided call stack and source code location.

convenience init(callStackAddresses: [NSNumber], location: XCTSourceCodeLocation?)

Initializes a new instance with an array of call stack addresses and a source code location.

convenience init(location: XCTSourceCodeLocation?)

Initializes a new instance with a call stack from the executing thread and a provided source code location.

convenience init()

Initializes a new instance with a call stack from the executing thread and no location.

### Context Information

var callStack: [XCTSourceCodeFrame]

An array of source code frames that describes the call stack when a test issue occurs.

var location: XCTSourceCodeLocation?

A representation of a location in source code where a test issue occurred.

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

class XCTSourceCodeFrame

An object that represents a single frame in a call stack that supports retrieval of symbol information for the address.

class XCTSourceCodeLocation

An object that contains a file URL and line number that represents a distinct location in source code.

class XCTSourceCodeSymbolInfo

An object that contains symbolication information for a specified frame in a call stack.

