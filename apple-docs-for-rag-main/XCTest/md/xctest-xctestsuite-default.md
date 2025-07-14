

- XCTest
- XCTestSuite
-  default 

Type Property

# default

Creates a suite of test suites that represents all test case methods in the current runtime.

``` source
class var `default`: XCTestSuite { get }
```

## See Also

### Creating Test Suites

init(name: String)

Creates a test suite with the specified name.

convenience init(forBundlePath: String)

Creates a test suite with the bundle at the specified path.

convenience init(forTestCaseClass: AnyClass)

Creates a test suite that contains all test methods in the specified class.

convenience init(forTestCaseWithName: String)

Creates a test suite that contains a test case with the specified name.

