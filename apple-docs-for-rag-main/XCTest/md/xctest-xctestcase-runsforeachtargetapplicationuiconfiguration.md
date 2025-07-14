

- XCTest
- XCTestCase
-  runsForEachTargetApplicationUIConfiguration 

Type Property

# runsForEachTargetApplicationUIConfiguration

A Boolean value that indicates whether your UI tests run once for each possible combination of orientation, localization, and other appearance settings your app supports.

``` source
class var runsForEachTargetApplicationUIConfiguration: Bool { get }
```

## Discussion

The default is `false`. Override this method to return `true` in your UI test case to run the tests once for each UI configuration your app supports. To determine what UI configurations your app supports, the test system examines your project settings, including:

- Appearance (for example, light mode or dark mode)

- Orientation (for example, portrait or landscape)

- Localization (for example, `en_US` or `zh_CN`)

The test system calculates a set of configurations that encompasses all the possible combinations of those supported settings, and provides each configuration to an iteration of your tests when you call launch() on XCUIApplication.

## See Also

### Managing Test Case Execution

var continueAfterFailure: Bool

A Boolean value that indicates whether a test method should continue running after a failure occurs.

var executionTimeAllowance: TimeInterval

The number of seconds, rounded up to the nearest minute, for a test to run before it fails with a timeout error.

