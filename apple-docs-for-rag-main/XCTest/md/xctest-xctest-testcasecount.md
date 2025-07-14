

- XCTest
- XCTest
-  testCaseCount 

Instance Property

# testCaseCount

The number of test cases in the test.

``` source
var testCaseCount: Int { get }
```

## Discussion

Must be overridden by subclasses.

## See Also

### Examining Test Properties

var name: String

The name of the test.

var testRun: XCTestRun?

The test run object that executes the test.

var testRunClass: AnyClass?

The test run subclass to instantiate when the test runs, which records the test’s results.

