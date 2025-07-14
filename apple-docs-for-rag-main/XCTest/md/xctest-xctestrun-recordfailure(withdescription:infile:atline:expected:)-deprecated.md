

- XCTest
- XCTestRun
-  recordFailure(withDescription:inFile:atLine:expected:) Deprecated

Instance Method

# recordFailure(withDescription:inFile:atLine:expected:)

Records a failure during test execution for the test run.

``` source
func recordFailure(
    withDescription description: String,
    inFile filePath: String?,
    atLine lineNumber: Int,
    expected: Bool
)
```

Deprecated

Use record(_:) instead.

## Parameters 

`description`  

The description of the failure.

`filePath`  

The file path to the source file where the failure occurred or `nil` if unknown.

`lineNumber`  

The line number in the source file at `filePath` where the failure occurred.

`expected`  

true if the failure was the result of a failed assertion, false if it was the result of an uncaught exception.

## Discussion

Don’t call this method before the test run starts or after it stops.

