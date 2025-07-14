

- XCTest
-  Comparable Value Assertions 

API Collection

# Comparable Value Assertions

Compare two values to determine whether one is larger or smaller than the other.

## Topics

### Tests for Comparable Values

func XCTAssertGreaterThan&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is greater than the value of the second expression.

func XCTAssertGreaterThanOrEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is greater than or equal to the value of the second expression.

func XCTAssertLessThanOrEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is less than or equal to the value of the second expression.

func XCTAssertLessThan&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is less than the value of the second expression.

## See Also

### Test assertions

Boolean Assertions

Test a condition that generates a true or false result.

Nil and Non-Nil Assertions

Check whether a test condition has, or doesn’t have, a value.

Equality and Inequality Assertions

Check whether two values are equal or unequal.

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

