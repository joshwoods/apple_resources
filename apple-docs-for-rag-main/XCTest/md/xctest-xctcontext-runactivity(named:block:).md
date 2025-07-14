

- XCTest
- XCTContext
-  runActivity(named:block:) 

Type Method

# runActivity(named:block:)

Creates and runs an activity with the provided block of code.

``` source
@MainActor @preconcurrency
class func runActivity(
    named name: String,
    block: @MainActor (any XCTActivity) throws -> Result
) rethrows -> Result
```

## Parameters 

`name`  

A descriptive name for the activity, for display in Xcode’s test results browser.

`block`  

A block of code for the test to execute as the body of the activity.

## Return Value

A Result object that indicates whether the block of code runs successfully or encounters an error.

## Discussion

Run a block of code as a named substep in a test. For more information, see Grouping Tests into Substeps with Activities.

To save screenshots or other test-result data for later investigation, call the add(_:) method on the instance of XCTActivity that the test system passes to your block. For more information, see Adding Attachments to Tests, Activities, and Issues.

## See Also

### Related Documentation

Grouping Tests into Substeps with Activities

Simplify test reports by creating activities that organize substeps within complex test methods.

Adding Attachments to Tests, Activities, and Issues

Use attachments to store a test’s output data for later analysis.

