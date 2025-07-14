

- XCTest
- XCTestRun
-  executionCount 

Instance Property

# executionCount

The number of test executions during the run.

``` source
var executionCount: Int { get }
```

## See Also

### Gathering Test Outcomes

var hasSucceeded: Bool

A Boolean value that returns true if all tests in the run completed without recording any failures; otherwise, false.

var hasBeenSkipped: Bool

A Boolean value that indicates a skipped test.

var failureCount: Int

The number of test failures during the run.

var skipCount: Int

The number of skipped tests during the run.

var test: XCTest

The test instance for the test run.

var testCaseCount: Int

The number of tests in the run.

var totalFailureCount: Int

The number of test failures and uncaught exceptions during the run.

var unexpectedExceptionCount: Int

The number of uncaught exceptions during the run.

