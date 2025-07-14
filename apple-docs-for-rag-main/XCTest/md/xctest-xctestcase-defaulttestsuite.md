

- XCTest
- XCTestCase
-  defaultTestSuite 

Type Property

# defaultTestSuite

A test suite that contains test cases for all of the tests in the class.

``` source
class var defaultTestSuite: XCTestSuite { get }
```

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

func recordFailure(withDescription: String, inFile: String, atLine: Int, expected: Bool)

Records a failure during text execution.

Deprecated

