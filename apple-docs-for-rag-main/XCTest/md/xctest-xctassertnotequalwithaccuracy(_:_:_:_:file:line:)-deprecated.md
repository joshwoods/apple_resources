

- XCTest
-  XCTAssertNotEqualWithAccuracy(\_:\_:\_:\_:file:line:) Deprecated

Function

# XCTAssertNotEqualWithAccuracy(\_:\_:\_:\_:file:line:)

Asserts that two values are not equal within a certain accuracy.

``` source
func XCTAssertNotEqualWithAccuracy(
    _ expression1: @autoclosure () throws -> T,
    _ expression2: @autoclosure () throws -> T,
    _ accuracy: T,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
) where T : FloatingPoint
```

Deprecated

Use XCTAssertNotEqual(_:_:accuracy:_:file:line:) instead.

## Parameters 

`expression1`  

An expression of type `T`, where `T` conforms to FloatingPoint.

`expression2`  

An expression of type `T`, where `T` conforms to FloatingPoint.

`accuracy`  

An expression of type `T`, where `T` conforms to FloatingPoint. Describes the maximum difference between `expression1` and `expression2` for these values to be considered not equal.

`message`  

An optional description of the failure.

`file`  

The file in which failure occurred. Defaults to the file name of the test case in which this function was called.

`line`  

The line number on which failure occurred. Defaults to the line number on which this function was called.

## Discussion

`expression1`, `expression2`, and `accuracy` must all be of the same type `T` that conforms to FloatingPoint.

## See Also

### Deprecated Functions

func XCTSelfTestMain() -> Int32Deprecated

func XCTAssertEqualWithAccuracy&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, accuracy: T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values are equal within a certain accuracy.

Deprecated

