

- XCTest
-  XCTAssertEqual(\_:\_:\_:file:line:) 

Function

# XCTAssertEqual(\_:\_:\_:file:line:)

Asserts that two values are equal.

``` source
func XCTAssertEqual(
    _ expression1: @autoclosure () throws -> T,
    _ expression2: @autoclosure () throws -> T,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
) where T : Equatable
```

## Parameters 

`expression1`  

An expression of type `T`, where `T` is `Equatable`.

`expression2`  

A second expression of type `T`, where `T` is `Equatable`.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## Discussion

Use this function to compare two non-optional values of the same type.

Listing 1. Comparing Non-Optional Values Of The Same Type

```
class FrameSizeTests: XCTestCase {
    func testInitialFrameSize() {
        let view = CustomView()
        let expectedSize = CGSize(width: 640.0, height: 480.0)
        XCTAssertEqual(view.frame.size, expectedSize, "Unexpected frame size.")
    }
}
```

Listing 1 creates a new instance of a custom class called `CustomView`, and checks that its size is equal to `CGSize(width: 640.0, height: 480.0)`.

## See Also

### Tests for Equality and Inequality

func XCTAssertNotEqual&lt;T>(@autoclosure () throws -> T, @autoclosure () throws -> T, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values are not equal.

