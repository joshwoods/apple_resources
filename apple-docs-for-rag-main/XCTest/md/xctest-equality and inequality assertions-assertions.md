

- XCTest
-  Equality and Inequality Assertions 

API Collection

# Equality and Inequality Assertions

Check whether two values are equal or unequal.

## Topics

### Tests for Equality and Inequality

func XCTAssertEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values are equal.

func XCTAssertNotEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values are not equal.

### Tests for Identical Objects

func XCTAssertIdentical(@autoclosure () throws -> AnyObject?, @autoclosure () throws -> AnyObject?, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values are identical.

func XCTAssertNotIdentical(@autoclosure () throws -> AnyObject?, @autoclosure () throws -> AnyObject?, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values aren’t identical.

### Tests for Equality Within a Specified Accuracy

func XCTAssertEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two floating-point values are equal within a specified accuracy.

func XCTAssertEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two numeric values are equal within a specified accuracy.

func XCTAssertNotEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two floating-point values aren’t equal within a specified accuracy.

func XCTAssertNotEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two numeric values aren’t equal within a specified accuracy.

## See Also

### Test assertions

Boolean Assertions

Test a condition that generates a true or false result.

Nil and Non-Nil Assertions

Check whether a test condition has, or doesn’t have, a value.

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

