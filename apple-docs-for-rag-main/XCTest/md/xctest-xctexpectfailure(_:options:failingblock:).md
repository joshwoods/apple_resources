

- XCTest
-  XCTExpectFailure(\_:options:failingBlock:) 

Function

# XCTExpectFailure(\_:options:failingBlock:)

Instructs the test to expect a failure in an assertion in the provided block of code, with options to customize expected failure checking and handling.

``` source
func XCTExpectFailure(
    _ failureReason: String? = nil,
    options: XCTExpectedFailure.Options = .init(),
    failingBlock: () throws -> R
) rethrows -> R
```

## Parameters 

`failureReason`  

An optional string that describes why the test expects a failure.

`options`  

Options that determine how the test matches the expected failure to an actual test failure, and whether an unfulfilled expected failure results in a test failure.

`failingBlock`  

A block of test code and assertions where the test expects a failure.

## Return Value

If the `failingBlock` you provide returns a value or throws an error, the function returns that value or rethrows the error.

## See Also

### Expected Failures

class XCTExpectedFailure

An object that represents an expected test failure.

class Options

Options that determine how the test matches the expected failure to an actual test failure, and whether an unfulfilled expected failure results in a test failure.

func XCTExpectFailure(String?, options: XCTExpectedFailure.Options)

Instructs the test to expect a failure in an upcoming assertion, with options to customize expected failure checking and handling.

func XCTExpectFailure(String?, enabled: Bool?, strict: Bool?, issueMatcher: ((XCTIssue) -> Bool)?)

Instructs the test to expect a failure in an upcoming assertion, with parameters to customize expected failure checking and handling.

func XCTExpectFailure&lt;R>(String?, enabled: Bool?, strict: Bool?, failingBlock: () throws -> R, issueMatcher: ((XCTIssue) -> Bool)?) rethrows -> R

Instructs the test to expect a failure in an assertion in the provided block of code, with parameters to customize expected failure checking and handling.

