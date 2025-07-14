

- XCTest
-  XCTSourceCodeLocation 

Class

# XCTSourceCodeLocation

An object that contains a file URL and line number that represents a distinct location in source code.

``` source
class XCTSourceCodeLocation
```

## Topics

### Initializers

init(fileURL: URL, lineNumber: Int)

Initializes a new instance with a file URL and a line number.

convenience init(filePath: String, lineNumber: Int)

Initializes a new instance with a file path and a line number.

convenience init(filePath: StaticString, lineNumber: UInt)

Initializes a new instance with a file path and a line number.

### Source Location Information

var fileURL: URL

A file URL that represents the file-system location of the source code file.

var lineNumber: Int

An integer that represents a line of code in a source code file.

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

class XCTSourceCodeSymbolInfo

An object that contains symbolication information for a specified frame in a call stack.

