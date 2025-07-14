

- XCTest
-  XCTAssertLessThanOrEqual(\_:\_:\_:file:line:) 

Function

# XCTAssertLessThanOrEqual(\_:\_:\_:file:line:)

Asserts that the value of the first expression is less than or equal to the value of the second expression.

``` source
func XCTAssertLessThanOrEqual(
    _ expression1: @autoclosure () throws -> T,
    _ expression2: @autoclosure () throws -> T,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
) where T : Comparable
```

## Parameters 

`expression1`  

An expression of type `T`, where `T` is Comparable.

`expression2`  

A second expression of type `T`, where `T` is Comparable.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## See Also

### Tests for Comparable Values

func XCTAssertGreaterThan&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is greater than the value of the second expression.

func XCTAssertGreaterThanOrEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is greater than or equal to the value of the second expression.

func XCTAssertLessThan&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that the value of the first expression is less than the value of the second expression.

