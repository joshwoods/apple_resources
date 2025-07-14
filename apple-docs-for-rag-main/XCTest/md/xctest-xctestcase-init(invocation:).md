

- XCTest
- XCTestCase
-  init(invocation:) 

Initializer

# init(invocation:)

Initializes a test case with an invocation.

``` source
init(invocation: NSInvocation?)
```

## Parameters 

`invocation`  

An invocation to use when running this test.

## See Also

### Creating Tests Programmatically

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

class var defaultTestSuite: XCTestSuite

A test suite that contains test cases for all of the tests in the class.

