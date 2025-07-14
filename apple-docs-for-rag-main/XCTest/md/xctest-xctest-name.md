

- XCTest
- XCTest
-  name 

Instance Property

# name

The name of the test.

``` source
var name: String { get }
```

## Discussion

Must be overridden by subclasses.

## See Also

### Examining Test Properties

var testCaseCount: Int

The number of test cases in the test.

var testRun: XCTestRun?

The test run object that executes the test.

var testRunClass: AnyClass?

The test run subclass to instantiate when the test runs, which records the test’s results.

