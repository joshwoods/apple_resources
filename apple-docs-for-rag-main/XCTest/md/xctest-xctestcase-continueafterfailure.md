

- XCTest
- XCTestCase
-  continueAfterFailure 

Instance Property

# continueAfterFailure

A Boolean value that indicates whether a test method should continue running after a failure occurs.

``` source
var continueAfterFailure: Bool { get set }
```

## Discussion

The default is true. Set this property to false within a test method to end execution of that method as soon as a failure occurs. Other test methods in the suite may still execute after a test fails.

## See Also

### Managing Test Case Execution

class var runsForEachTargetApplicationUIConfiguration: Bool

A Boolean value that indicates whether your UI tests run once for each possible combination of orientation, localization, and other appearance settings your app supports.

var executionTimeAllowance: TimeInterval

The number of seconds, rounded up to the nearest minute, for a test to run before it fails with a timeout error.

