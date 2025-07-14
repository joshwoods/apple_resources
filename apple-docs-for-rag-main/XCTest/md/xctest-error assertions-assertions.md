

- XCTest
-  Error Assertions 

API Collection

# Error Assertions

Check whether a function call throws, or doesn’t throw, an error.

## Topics

### Tests for Errors

func XCTAssertThrowsError&lt;T>(@autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt, (any Error) -> Void)

Asserts that an expression throws an error.

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

NSException Assertions

Check whether a function call throws, or doesn’t throw, an exception.

Unconditional Test Failures

Generate a failure immediately and unconditionally.

Expected Failures

Anticipate known test failures to prevent failing tests from affecting your workflows.

Methods for Skipping Tests

Skip tests when meeting specified conditions.

