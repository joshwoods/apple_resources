

- XCTest
- XCTestSuite
-  init(forTestCaseWithName:) 

Initializer

# init(forTestCaseWithName:)

Creates a test suite that contains a test case with the specified name.

``` source
convenience init(forTestCaseWithName name: String)
```

## Parameters 

`name`  

A string that specifies a test case.

## See Also

### Creating Test Suites

class var `default`: XCTestSuite

Creates a suite of test suites that represents all test case methods in the current runtime.

init(name: String)

Creates a test suite with the specified name.

convenience init(forBundlePath: String)

Creates a test suite with the bundle at the specified path.

convenience init(forTestCaseClass: AnyClass)

Creates a test suite that contains all test methods in the specified class.

