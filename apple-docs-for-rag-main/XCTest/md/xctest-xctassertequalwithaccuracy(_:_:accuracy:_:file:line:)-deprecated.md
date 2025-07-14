

- XCTest
-  XCTAssertEqualWithAccuracy(\_:\_:accuracy:\_:file:line:) Deprecated

Function

# XCTAssertEqualWithAccuracy(\_:\_:accuracy:\_:file:line:)

Asserts that two values are equal within a certain accuracy.

``` source
func XCTAssertEqualWithAccuracy(
    _ expression1: @autoclosure () throws -> T,
    _ expression2: @autoclosure () throws -> T,
    accuracy: T,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
) where T : FloatingPoint
```

Deprecated

Use XCTAssertEqual(_:_:accuracy:_:file:line:) instead.

## Parameters 

`expression1`  

An expression of type `T`, where `T` conforms to FloatingPoint.

`expression2`  

An expression of type `T`, where `T` conforms to FloatingPoint.

`accuracy`  

An expression of type `T`, where `T` conforms to FloatingPoint. Describes the maximum difference between `expression1` and `expression2` for these values to be considered equal.

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

func XCTAssertNotEqualWithAccuracy&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values are not equal within a certain accuracy.

Deprecated

