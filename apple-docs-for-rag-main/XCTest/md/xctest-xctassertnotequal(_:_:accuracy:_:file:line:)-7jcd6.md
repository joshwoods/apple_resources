

- XCTest
-  XCTAssertNotEqual(\_:\_:accuracy:\_:file:line:) 

Function

# XCTAssertNotEqual(\_:\_:accuracy:\_:file:line:)

Asserts that two floating-point values aren’t equal within a specified accuracy.

``` source
func XCTAssertNotEqual(
    _ expression1: @autoclosure () throws -> T,
    _ expression2: @autoclosure () throws -> T,
    accuracy: T,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
) where T : FloatingPoint
```

## Parameters 

`expression1`  

An expression of type `T`, where `T` conforms to FloatingPoint.

`expression2`  

A second expression of type `T`, where `T` conforms to FloatingPoint.

`accuracy`  

An expression of type `T`, where `T` conforms to FloatingPoint. This parameter describes the maximum difference between `expression1` and `expression2` for these values to be considered not equal.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## Discussion

`expression1`, `expression2`, and `accuracy` must all be of the same type `T`, and type `T` must conform to FloatingPoint.

## See Also

### Tests for Equality Within a Specified Accuracy

func XCTAssertEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two floating-point values are equal within a specified accuracy.

func XCTAssertEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two numeric values are equal within a specified accuracy.

func XCTAssertNotEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two numeric values aren’t equal within a specified accuracy.

