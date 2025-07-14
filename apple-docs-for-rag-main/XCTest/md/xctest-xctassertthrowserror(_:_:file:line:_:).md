

- XCTest
-  XCTAssertThrowsError(\_:\_:file:line:\_:) 

Function

# XCTAssertThrowsError(\_:\_:file:line:\_:)

Asserts that an expression throws an error.

``` source
func XCTAssertThrowsError(
    _ expression: @autoclosure () throws -> T,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line,
    _ errorHandler: (any Error) -> Void = { _ in }
)
```

## Parameters 

`expression`  

An expression that can throw an error.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

`errorHandler`  

An optional handler for errors that `expression` throws.

