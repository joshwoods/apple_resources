

- XCTest
- XCTestCase
-  testInvocations 

Type Property

# testInvocations

An array of invocations that represents each test method in the test case.

``` source
class var testInvocations: [NSInvocation] { get }
```

## See Also

### Creating Tests Programmatically

init(invocation: NSInvocation?)

Initializes a test case with an invocation.

init(selector: Selector)

Initializes a test case with a selector.

var invocation: NSInvocation?

The invocation for running the test.

func invokeTest()

Invokes the test.

func record(XCTIssue)

Records an issue during test execution.

func recordFailure(withDescription: String, inFile: String, atLine: Int, expected: Bool)

Records a failure during text execution.

Deprecated

class var defaultTestSuite: XCTestSuite

A test suite that contains test cases for all of the tests in the class.

