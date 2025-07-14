

- XCTest
- XCTExpectedFailure
-  XCTExpectedFailure.Options 

Class

# XCTExpectedFailure.Options

Options that determine how the test matches the expected failure to an actual test failure, and whether an unfulfilled expected failure results in a test failure.

``` source
class Options
```

## Overview

Create options and provide them to `XCTExpectFailure` functions to tell the test system how to match an expected failure, whether to enable an expected failure during a test, and whether an unfulfilled expected failure generates a test failure.

## Topics

### Matching Failures

var issueMatcher: (XCTIssue) -> Bool

A block of code that determines whether the test issue fulfills the expected failure.

### Specifying Options

class func nonStrict() -> XCTExpectedFailure.Options

Options that specify that an unfulfilled expected failure doesn’t generate a test failure.

var isEnabled: Bool

A Boolean value that indicates whether the test checks for the expected failure.

var isStrict: Bool

A Boolean value that indicates whether the test reports an error if the expected failure doesn’t occur.

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
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Expected Failures

class XCTExpectedFailure

An object that represents an expected test failure.

func XCTExpectFailure(String?, options: XCTExpectedFailure.Options)

Instructs the test to expect a failure in an upcoming assertion, with options to customize expected failure checking and handling.

func XCTExpectFailure(String?, enabled: Bool?, strict: Bool?, issueMatcher: ((XCTIssue) -> Bool)?)

Instructs the test to expect a failure in an upcoming assertion, with parameters to customize expected failure checking and handling.

func XCTExpectFailure&lt;R>(String?, options: XCTExpectedFailure.Options, failingBlock: () throws -> R) rethrows -> R

Instructs the test to expect a failure in an assertion in the provided block of code, with options to customize expected failure checking and handling.

func XCTExpectFailure&lt;R>(String?, enabled: Bool?, strict: Bool?, failingBlock: () throws -> R, issueMatcher: ((XCTIssue) -> Bool)?) rethrows -> R

Instructs the test to expect a failure in an assertion in the provided block of code, with parameters to customize expected failure checking and handling.

