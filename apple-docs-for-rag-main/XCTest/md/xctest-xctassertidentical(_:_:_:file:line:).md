

- XCTest
-  XCTAssertIdentical(\_:\_:\_:file:line:) 

Function

# XCTAssertIdentical(\_:\_:\_:file:line:)

Asserts that two values are identical.

``` source
func XCTAssertIdentical(
    _ expression1: @autoclosure () throws -> AnyObject?,
    _ expression2: @autoclosure () throws -> AnyObject?,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
)
```

## Parameters 

`expression1`  

An optional expression of type AnyObject.

`expression2`  

A second optional expression of type AnyObject.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## Discussion

Compare two optional values of types that conform to `AnyObject`. The values are identical if they’re the same instance.

## See Also

### Tests for Identical Objects

func XCTAssertNotIdentical(@autoclosure () throws -> AnyObject?, @autoclosure () throws -> AnyObject?, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that two values aren’t identical.

