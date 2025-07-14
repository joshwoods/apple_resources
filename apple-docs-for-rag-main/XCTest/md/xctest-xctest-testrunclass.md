

- XCTest
- XCTest
-  testRunClass 

Instance Property

# testRunClass

The test run subclass to instantiate when the test runs, which records the test’s results.

``` source
var testRunClass: AnyClass? { get }
```

## Discussion

Subclasses must override `testRunClass`.

## See Also

### Examining Test Properties

var name: String

The name of the test.

var testCaseCount: Int

The number of test cases in the test.

var testRun: XCTestRun?

The test run object that executes the test.

