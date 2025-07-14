

- Swift Testing
-  expect(\_:sourceLocation:performing:throws:) Deprecated

Macro

# expect(\_:sourceLocation:performing:throws:)

Check that an expression always throws an error matching some condition.

Swift 6.0+Xcode 16.0+

``` source
@discardableResult @freestanding(expression)
macro expect(
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation,
    performing expression: () async throws -> R,
    throws errorMatcher: (any Error) async throws -> Bool
) -> (any Error)?
```

Deprecated

Examine the result of expect(throws:_:sourceLocation:performing:) or expect(throws:_:sourceLocation:performing:) instead:

```
let error = #expect(throws: FoodTruckError.self) {
  ...
}
#expect(error?.napkinCount == 0)
```

## See Also

### Checking that errors are thrown

Testing for errors in Swift code

Ensure that your code handles errors in the way you expect.

macro expect&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws an error of a given type.

macro expect&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws a specific error.

macro require&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

Check that an expression always throws an error of a given type, and throw an error if it does not.

macro require&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

macro require&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> any Error

Check that an expression always throws an error matching some condition, and throw an error if it does not.

Deprecated

