

- XCTest
- XCTestRun
-  stop() 

Instance Method

# stop()

Stops a test run.

``` source
func stop()
```

## Discussion

This method must not be called unless the run has been started, and must not be called more than once.

## See Also

### Performing Test Runs

func start()

Starts a test run.

func record(XCTIssue)

Records an issue during test execution for the test run.

