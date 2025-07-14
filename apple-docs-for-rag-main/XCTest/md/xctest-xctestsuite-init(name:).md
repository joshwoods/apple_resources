

- XCTest
- XCTestSuite
-  init(name:) 

Initializer

# init(name:)

Creates a test suite with the specified name.

``` source
init(name: String)
```

## Parameters 

`name`  

The name of the test.

## See Also

### Creating Test Suites

class var `default`: XCTestSuite

Creates a suite of test suites that represents all test case methods in the current runtime.

convenience init(forBundlePath: String)

Creates a test suite with the bundle at the specified path.

convenience init(forTestCaseClass: AnyClass)

Creates a test suite that contains all test methods in the specified class.

convenience init(forTestCaseWithName: String)

Creates a test suite that contains a test case with the specified name.

