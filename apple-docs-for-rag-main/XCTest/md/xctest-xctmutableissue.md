

- XCTest
-  XCTMutableIssue 

Class

# XCTMutableIssue

A mutable object that represents a test failure, and includes source code call stacks for test reporting and investigation.

``` source
class XCTMutableIssue
```

## Topics

### Issue Details

var type: XCTIssueReference.IssueType

A value for classifying an issue that occurs during testing.

var compactDescription: String

A concise description of the issue with no transient data, suitable for use in test run summaries and results aggregation across multiple test runs.

var detailedDescription: String?

A detailed description of the issue that may include transient data, such as numbers, object identifiers, and timestamps, to help diagnose the issue.

var sourceCodeContext: XCTSourceCodeContext

The source code location for the issue, including the filename, line number, and call stack.

var associatedError: (any Error)?

An optional error to associate with a test issue.

var attachments: [XCTAttachment]

An array of data that augments an issue, such as files, images, screenshots, data blobs, or ZIP files.

func add(XCTAttachment)

Adds supporting data to an issue.

## Relationships

### Inherits From

- XCTIssueReference

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Test Failures

struct XCTIssue

An object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTIssueReference

An object that represents a test failure, and includes source code call stacks for test reporting and investigation.

class XCTSourceCodeContext

An object that contains call stack and source code location details to provide context for a point of execution in a test.

class XCTSourceCodeFrame

An object that represents a single frame in a call stack that supports retrieval of symbol information for the address.

class XCTSourceCodeLocation

An object that contains a file URL and line number that represents a distinct location in source code.

class XCTSourceCodeSymbolInfo

An object that contains symbolication information for a specified frame in a call stack.

