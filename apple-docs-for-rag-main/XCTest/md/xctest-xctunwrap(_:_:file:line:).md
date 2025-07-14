

- XCTest
-  XCTUnwrap(\_:\_:file:line:) 

Function

# XCTUnwrap(\_:\_:file:line:)

Asserts that an expression is not `nil,` and returns the unwrapped value.

``` source
func XCTUnwrap(
    _ expression: @autoclosure () throws -> T?,
    _ message: @autoclosure () -> String = "",
    file: StaticString = #filePath,
    line: UInt = #line
) throws -> T
```

## Parameters 

`expression`  

An expression of type `T?`. The expression’s type determines the type of the return value.

`message`  

An optional description of a failure.

`file`  

The file where the failure occurs. The default is the filename of the test case where you call this function.

`line`  

The line number where the failure occurs. The default is the line number where you call this function.

## Return Value

The result of evaluating and unwrapping the `expression`, which is of type `T`. `XCTUnwrap()` only returns a value if `expression` is not `nil`.

## Discussion

This function generates a failure when `expression` is `nil`. Otherwise, it returns the unwrapped value of `expression` for subsequent use in the test.

## See Also

### Tests for a Non-Nil Condition

func XCTAssertNotNil(@autoclosure () throws -> Any?, @autoclosure () -> String, file: StaticString, line: UInt)

Asserts that an expression is not `nil`.

