

- XCTest
-  Nil and Non-Nil Assertions 

API Collection

# Nil and Non-Nil Assertions

Check whether a test condition has, or doesn’t have, a value.

## Topics

### Tests for a Nil Condition

func XCTAssertNil(@autoclosure () throws -> Any?, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that an expression is `nil`.

### Tests for a Non-Nil Condition

func XCTAssertNotNil(@autoclosure () throws -> Any?, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that an expression is not `nil`.

func XCTUnwrap&lt;T>(@autoclosure () throws -> T?, @autoclosure () -> String, file: StaticString, line: UInt) throws -> T

Asserts that an expression is not `nil,` and returns the unwrapped value.

## See Also

### Test assertions

Boolean Assertions

Test a condition that generates a true or false result.

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

Methods for Skipping Tests

Skip tests when meeting specified conditions.

