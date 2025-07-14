

- XCTest
-  XCTAssertNotNil(\_:\_:file:line:) 

Function

# XCTAssertNotNil(\_:\_:file:line:)

Asserts that an expression is not `nil`.

``` source
func XCTAssertNotNil(
    _ expression: @autoclosure () throws -> Any?,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
)
```

## Parameters 

`expression`  

An expression of type `Any?` to compare against `nil`.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## Discussion

This function generates a failure when `expression == nil`.

## See Also

### Tests for a Non-Nil Condition

func XCTUnwrap&lt;T>(@autoclosure () throws -> T?, @autoclosure () -> String, file: StaticString, line: UInt) throws -> T

Asserts that an expression is not `nil,` and returns the unwrapped value.

