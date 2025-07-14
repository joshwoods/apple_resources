

- XCTest
-  XCTAssertFalse(\_:\_:file:line:) 

Function

# XCTAssertFalse(\_:\_:file:line:)

Asserts that an expression is false.

``` source
func XCTAssertFalse(
    _ expression: @autoclosure () throws -> Bool,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
)
```

## Parameters 

`expression`  

An expression of Boolean type.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## Discussion

This function generates a failure when `expression == true`.

