

- XCTest
- XCTestSuite
-  init(forTestCaseClass:) 

Initializer

# init(forTestCaseClass:)

Creates a test suite that contains all test methods in the specified class.

``` source
convenience init(forTestCaseClass testCaseClass: AnyClass)
```

## Parameters 

`testCaseClass`  

A class that contains test cases.

## See Also

### Creating Test Suites

class var `default`: XCTestSuite

Creates a suite of test suites that represents all test case methods in the current runtime.

init(name: String)

Creates a test suite with the specified name.

convenience init(forBundlePath: String)

Creates a test suite with the bundle at the specified path.

convenience init(forTestCaseWithName: String)

Creates a test suite that contains a test case with the specified name.

