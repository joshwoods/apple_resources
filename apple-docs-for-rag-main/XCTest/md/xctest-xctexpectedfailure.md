

- XCTest
-  XCTExpectedFailure 

Class

# XCTExpectedFailure

An object that represents an expected test failure.

``` source
class XCTExpectedFailure
```

## Overview

The test system creates and tracks instances of `XCTExpectedFailure` when you call one of the `XCTExpectFailure` functions. Don’t create or use them directly.

## Topics

### Detailing Expected Failure

var failureReason: String?

An optional string that describes why the test expects a failure.

var issue: XCTIssue

The issue that fulfills the expected failure.

### Setting Options

class Options

Options that determine how the test matches the expected failure to an actual test failure, and whether an unfulfilled expected failure results in a test failure.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Expected Failures

class Options

Options that determine how the test matches the expected failure to an actual test failure, and whether an unfulfilled expected failure results in a test failure.

func XCTExpectFailure(String?, options: XCTExpectedFailure.Options)

Instructs the test to expect a failure in an upcoming assertion, with options to customize expected failure checking and handling.

func XCTExpectFailure(String?, enabled: Bool?, strict: Bool?, issueMatcher: ((XCTIssue) -> Bool)?)

Instructs the test to expect a failure in an upcoming assertion, with parameters to customize expected failure checking and handling.

func XCTExpectFailure&lt;R>(String?, options: XCTExpectedFailure.Options, failingBlock: () throws -> R) rethrows -> R

Instructs the test to expect a failure in an assertion in the provided block of code, with options to customize expected failure checking and handling.

func XCTExpectFailure&lt;R>(String?, enabled: Bool?, strict: Bool?, failingBlock: () throws -> R, issueMatcher: ((XCTIssue) -> Bool)?) rethrows -> R

Instructs the test to expect a failure in an assertion in the provided block of code, with parameters to customize expected failure checking and handling.

