

- XCTest
- XCTIssueReference
-  XCTIssueReference.IssueType 

Enumeration

# XCTIssueReference.IssueType

Constants that indicate types of test failures, such as assertion failures, performance regressions, or thrown errors.

``` source
enum IssueType
```

## Topics

### Issue Types

case assertionFailure

A test failure due to a failed test assertion or related API.

case performanceRegression

A test failure due to a performance regression.

case system

A test failure due to an internal failure in the testing framework.

case thrownError

A test failure when the test throws an error in Swift.

case uncaughtException

A test failure when code throws an exception and doesn’t catch it.

case unmatchedExpectedFailure

A test failure due to an expected test failure that doesn’t occur.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

