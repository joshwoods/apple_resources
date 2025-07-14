

- XCTest
-  XCTSkip 

Structure

# XCTSkip

An error that causes the current test to cease executing and the test runner to mark the test as skipped when the test throws the error.

``` source
struct XCTSkip
```

## Topics

### Skipping a Test

init(String?, file: StaticString, line: UInt)

Intitializes an error to skip a test.

### Describing a Skipped Test

var message: String?

An optional description of the skipped test, displayed in the Test navigator.

## Relationships

### Conforms To

- CustomNSError
- Error
- Sendable

## See Also

### Methods for Skipping Tests

func XCTSkipIf(@autoclosure () throws -> Bool, @autoclosure () -> String?, file: StaticString, line: UInt) throws

Skips remaining tests in a test method if the specified condition is met.

func XCTSkipUnless(@autoclosure () throws -> Bool, @autoclosure () -> String?, file: StaticString, line: UInt) throws

Skips remaining tests in a test method unless the specified condition is met.

