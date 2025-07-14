

- XCTest
- XCTestExpectation
-  init(description:) 

Initializer

# init(description:)

Creates a new XCTestExpectation with the provided description.

``` source
init(description expectationDescription: String)
```

## Parameters 

`expectationDescription`  

A string to display in the test log for this expectation, to help diagnose failures.

## Discussion

To fulfill an expectation that was created with this initializer, call the expectation’s fulfill() method when the asynchronous task in your test has completed.

## See Also

### Creating Expectations

var expectationDescription: String

A human readable string used to describe the expectation in log output and test reports.

