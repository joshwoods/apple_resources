

- XCTest
- XCTestCase
-  record(\_:) 

Instance Method

# record(\_:)

Records an issue during test execution.

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

func recordFailure(withDescription: String, inFile: String, atLine: Int, expected: Bool)

Records a failure during text execution.

Deprecated

class var defaultTestSuite: XCTestSuite

A test suite that contains test cases for all of the tests in the class.

