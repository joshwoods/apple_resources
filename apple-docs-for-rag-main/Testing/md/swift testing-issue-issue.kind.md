

- Swift Testing
- Issue
-  Issue.Kind 

Enumeration

# Issue.Kind

Kinds of issues which may be recorded.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
enum Kind
```

## Topics

### Enumeration Cases

case apiMisused

An issue occurred due to misuse of the testing library.

case confirmationMiscounted(actual: Int, expected: any RangeExpression &amp; Sendable)

An issue due to a confirmation being confirmed the wrong number of times.

case errorCaught(any Error)

An issue due to an `Error` being thrown by a test function and caught by the testing library.

case expectationFailed(Expectation)

An issue due to a failed expectation, such as those produced by expect(_:_:sourceLocation:).

case knownIssueNotRecorded

A known issue was expected, but was not recorded.

case system

An issue due to a failure in the underlying system, not due to a failure within the tests being run.

case timeLimitExceeded(timeLimitComponents: (seconds: Int64, attoseconds: Int64))

An issue due to a test reaching its time limit and timing out.

case unconditional

An issue which occurred unconditionally, for example by using record(_:sourceLocation:).

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

