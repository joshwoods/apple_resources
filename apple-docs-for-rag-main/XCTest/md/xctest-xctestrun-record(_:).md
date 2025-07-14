

- XCTest
- XCTestRun
-  record(\_:) 

Instance Method

# record(\_:)

Records an issue during test execution for the test run.

**macOS**

``` source
func record(_ issue: XCTIssueReference)
```

**iOS, iPadOS, tvOS, visionOS, watchOS**

``` source
func record(_ issue: XCTIssue)
```

## Parameters 

`issue`  

The test issue to record.

## Discussion

The test run records a failure or other issue during test execution with this method. Override to customize the issue, and call `super` unless you want to suppress the issue.

## See Also

### Performing Test Runs

func start()

Starts a test run.

func stop()

Stops a test run.

