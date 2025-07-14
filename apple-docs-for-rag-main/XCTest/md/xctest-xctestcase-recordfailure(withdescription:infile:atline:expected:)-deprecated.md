

- XCTest
- XCTestCase
-  recordFailure(withDescription:inFile:atLine:expected:) Deprecated

Instance Method

# recordFailure(withDescription:inFile:atLine:expected:)

Records a failure during text execution.

``` source
func recordFailure(
    withDescription description: String,
    inFile filePath: String,
    atLine lineNumber: Int,
    expected: Bool
)
```

Deprecated

Use record(_:) instead.

## Parameters 

`description`  

A description of the failure.

`filePath`  

The file path to the source file where the failure occurred.

`lineNumber`  

The line number in the source file at `filePath` where the failure occurred.

`expected`  

true if the failure was the result of a failed assertion, false if it was the result of an uncaught exception.

## Discussion

All test assertions use this method to record test failures.

## See Also

### Creating Tests Programmatically

init(invocation: NSInvocation?)

Initializes a test case with an invocation.

init(selector: Selector)

Initializes a test case with a selector.

class var testInvocations: [NSInvocation]

An array of invocations that represents each test method in the test case.

var invocation: NSInvocation?

The invocation for running the test.

func invokeTest()

Invokes the test.

func record(XCTIssue)

Records an issue during test execution.

class var defaultTestSuite: XCTestSuite

A test suite that contains test cases for all of the tests in the class.

