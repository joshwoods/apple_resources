

- XCTest
- XCTIssueReference
- XCTIssueReference.IssueType
-  XCTIssueReference.IssueType.thrownError 

Case

# XCTIssueReference.IssueType.thrownError

A test failure when the test throws an error in Swift.

``` source
case thrownError
```

## Discussion

This could also occur if an Objective-C test uses the form `-(BOOL)testExample:(NSError **)outError` and returns `NO` with a non-`nil` out error.

## See Also

### Issue Types

case assertionFailure

A test failure due to a failed test assertion or related API.

case performanceRegression

A test failure due to a performance regression.

case system

A test failure due to an internal failure in the testing framework.

case uncaughtException

A test failure when code throws an exception and doesn’t catch it.

case unmatchedExpectedFailure

A test failure due to an expected test failure that doesn’t occur.

