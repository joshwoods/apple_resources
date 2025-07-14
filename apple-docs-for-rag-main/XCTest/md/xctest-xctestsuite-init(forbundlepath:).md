

- XCTest
- XCTestSuite
-  init(forBundlePath:) 

Initializer

# init(forBundlePath:)

Creates a test suite with the bundle at the specified path.

``` source
convenience init(forBundlePath bundlePath: String)
```

## Parameters 

`bundlePath`  

A string that represents a file path to a bundle.

## See Also

### Creating Test Suites

class var `default`: XCTestSuite

Creates a suite of test suites that represents all test case methods in the current runtime.

init(name: String)

Creates a test suite with the specified name.

convenience init(forTestCaseClass: AnyClass)

Creates a test suite that contains all test methods in the specified class.

convenience init(forTestCaseWithName: String)

Creates a test suite that contains a test case with the specified name.

