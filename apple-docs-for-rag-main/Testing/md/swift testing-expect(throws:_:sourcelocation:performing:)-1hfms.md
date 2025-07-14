

- Swift Testing
-  expect(throws:\_:sourceLocation:performing:) 

Macro

# expect(throws:\_:sourceLocation:performing:)

Check that an expression always throws an error of a given type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@discardableResult @freestanding(expression)
macro expect(
    throws errorType: E.Type,
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation,
    performing expression: () async throws -> R
) -> E? where E : Error
```

## Parameters 

`errorType`  

The type of error that is expected to be thrown. If `expression` could throw *any* error, or the specific type of thrown error is unimportant, pass `(any Error).self`.

`comment`  

A comment describing the expectation.

`sourceLocation`  

The source location to which recorded expectations and issues should be attributed.

`expression`  

The expression to be evaluated.

## Return Value

If the expectation passes, the instance of `errorType` that was thrown by `expression`. If the expectation fails, the result is `nil`.

## Overview

Use this overload of `#expect()` when the expression `expression` *should* throw an error of a given type:

```
#expect(throws: EngineFailureError.self) {
  FoodTruck.shared.engine.batteryLevel = 0
  try FoodTruck.shared.engine.start()
}
```

If `expression` does not throw an error, or if it throws an error that is not an instance of `errorType`, an Issue is recorded for the test that is running in the current task. Any value returned by `expression` is discarded.

If the thrown error need only equal another instance of Error, use expect(throws:_:sourceLocation:performing:) instead.

## Expressions that should never throw

If the expression `expression` should *never* throw any error, you can pass Never.self:

```
#expect(throws: Never.self) {
  FoodTruck.shared.engine.batteryLevel = 100
  try FoodTruck.shared.engine.start()
}
```

If `expression` throws an error, an Issue is recorded for the test that is running in the current task. Any value returned by `expression` is discarded.

Test functions can be annotated with `throws` and can throw errors which are then recorded as issues when the test runs. If the intent is for a test to fail when an error is thrown by `expression`, rather than to explicitly check that an error is *not* thrown by it, do not use this macro. Instead, simply call the code in question and allow it to throw an error naturally.

## See Also

### Checking that errors are thrown

Testing for errors in Swift code

Ensure that your code handles errors in the way you expect.

macro expect&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws a specific error.

macro expect&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> (any Error)?

Check that an expression always throws an error matching some condition.

Deprecated

macro require&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

Check that an expression always throws an error of a given type, and throw an error if it does not.

macro require&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

macro require&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> any Error

Check that an expression always throws an error matching some condition, and throw an error if it does not.

Deprecated

