

- XCTest
-  Boolean Assertions 

API Collection

# Boolean Assertions

Test a condition that generates a true or false result.

## Topics

### Tests for True Conditions

func XCTAssert(@autoclosure () throws -> Bool, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that an expression is true.

func XCTAssertTrue(@autoclosure () throws -> Bool, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that an expression is true.

### Tests for False Conditions

func XCTAssertFalse(@autoclosure () throws -> Bool, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that an expression is false.

## See Also

### Test assertions

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

Methods for Skipping Tests

Skip tests when meeting specified conditions.

