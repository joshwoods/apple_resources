

- XCTest
- XCTestCase
-  invokeTest() 

Instance Method

# invokeTest()

Invokes the test.

``` source
func invokeTest()
```

## Discussion

Invoking a test performs its setup, invocation, and teardown. In general this should not be called directly.

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

func record(XCTIssue)

Records an issue during test execution.

func recordFailure(withDescription: String, inFile: String, atLine: Int, expected: Bool)

Records a failure during text execution.

Deprecated

class var defaultTestSuite: XCTestSuite

A test suite that contains test cases for all of the tests in the class.

