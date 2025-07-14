

- XCTest
- XCTest
-  testRun 

Instance Property

# testRun

The test run object that executes the test.

``` source
var testRun: XCTestRun? { get }
```

## Discussion

An instance of testRunClass, or `nil` if the test hasn’t run.

## See Also

### Examining Test Properties

var name: String

The name of the test.

var testCaseCount: Int

The number of test cases in the test.

var testRunClass: AnyClass?

The test run subclass to instantiate when the test runs, which records the test’s results.

