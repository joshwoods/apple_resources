

- XCTest
-  XCTestLog Deprecated

Class

# XCTestLog

An object that logs test failures and errors.

``` source
class XCTestLog
```

Deprecated

Use XCTIssue instead.

## Topics

### Logging Test Results

var logFileHandle: FileHandle!

An object to interact with the test log file.

func testLog(withFormat: String!, arguments: CVaListPointer)

Logs test results to the test log.

## Relationships

### Inherits From

- XCTestObserver

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Deprecated Classes

class XCTestObserver

An object that observes test activity and events.

Deprecated

class XCTestProbe

An object that observes test activity status.

Deprecated

