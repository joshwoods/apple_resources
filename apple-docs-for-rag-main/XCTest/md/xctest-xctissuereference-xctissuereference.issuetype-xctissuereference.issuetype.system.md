

- XCTest
- XCTIssueReference
- XCTIssueReference.IssueType
-  XCTIssueReference.IssueType.system 

Case

# XCTIssueReference.IssueType.system

A test failure due to an internal failure in the testing framework.

``` source
case system
```

## Discussion

This type of failure could happen if `XCUIApplication` was unable to launch or terminate an app, or if `XCUIElementQuery` was unable to complete a query.

## See Also

### Issue Types

case assertionFailure

A test failure due to a failed test assertion or related API.

case performanceRegression

A test failure due to a performance regression.

case thrownError

A test failure when the test throws an error in Swift.

case uncaughtException

A test failure when code throws an exception and doesn’t catch it.

case unmatchedExpectedFailure

A test failure due to an expected test failure that doesn’t occur.

