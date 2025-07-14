

- XCTest
-  Methods for Skipping Tests 

API Collection

# Methods for Skipping Tests

Skip tests when meeting specified conditions.

## Overview

Use `XCTSkipIf()` or `XCTSkipUnless()` when you have a Boolean condition that you can use to evaluate when to skip tests.

In Swift, throw an `XCTSkip` error when you have other circumstances that result in skipped tests. In Objective-C use `XCTSkip`. For example:

- Swift
- Objective-C

```
func testSomethingNew() throws {
    guard #available(macOS , *) else {
        throw XCTSkip("Required API is not available for this test.")
    }
    // perform test using  APIs...
}
```

```
- (void)testSomethingNew {
    if (@available(macOS , *)) {
        // perform test using  APIs...
    } else {
        XCTSkip(@"Required API is not available for this test.");
    }
}
```

## Topics

### Methods for Skipping Tests

func XCTSkipIf(@autoclosure () throws -> Bool, @autoclosure () -> String?, file: StaticString, line: UInt) throws

Skips remaining tests in a test method if the specified condition is met.

func XCTSkipUnless(@autoclosure () throws -> Bool, @autoclosure () -> String?, file: StaticString, line: UInt) throws

Skips remaining tests in a test method unless the specified condition is met.

struct XCTSkip

An error that causes the current test to cease executing and the test runner to mark the test as skipped when the test throws the error.

## See Also

### Test assertions

Boolean Assertions

Test a condition that generates a true or false result.

Nil and Non-Nil Assertions

Check whether a test condition has, or doesn’t have, a value.

Equality and Inequality Assertions

Check whether two values are equal or unequal.

Comparable Value Assertions

Compare two values to determine whether one is larger or smaller than the other.

Error Assertions

Check whether a function call throws, or doesn’t throw, an error.

NSException Assertions

Check whether a function call throws, or doesn’t throw, an exception.

Unconditional Test Failures

Generate a failure immediately and unconditionally.

Expected Failures

Anticipate known test failures to prevent failing tests from affecting your workflows.

