

- Swift Testing
-  expect(throws:\_:sourceLocation:performing:) 

Macro

# expect(throws:\_:sourceLocation:performing:)

Check that an expression always throws a specific error.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@discardableResult @freestanding(expression)
macro expect(
    throws error: E,
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation,
    performing expression: () async throws -> R
) -> E? where E : Equatable, E : Error
```

## Parameters 

`error`  

The error that is expected to be thrown.

`comment`  

A comment describing the expectation.

`sourceLocation`  

The source location to which recorded expectations and issues should be attributed.

`expression`  

The expression to be evaluated.

## Return Value

If the expectation passes, the instance of `E` that was thrown by `expression` and is equal to `error`. If the expectation fails, the result is `nil`.

## Mentioned in 

Testing for errors in Swift code

## Overview

Use this overload of `#expect()` when the expression `expression` *should* throw a specific error:

```
#expect(throws: EngineFailureError.batteryDied) {
  FoodTruck.shared.engine.batteryLevel = 0
  try FoodTruck.shared.engine.start()
}
```

If `expression` does not throw an error, or if it throws an error that is not equal to `error`, an Issue is recorded for the test that is running in the current task. Any value returned by `expression` is discarded.

If the thrown error need only be an instance of a particular type, use expect(throws:_:sourceLocation:performing:) instead.

## See Also

### Checking that errors are thrown

Testing for errors in Swift code

Ensure that your code handles errors in the way you expect.

macro expect&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws an error of a given type.

macro expect&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> (any Error)?

Check that an expression always throws an error matching some condition.

Deprecated

macro require&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

Check that an expression always throws an error of a given type, and throw an error if it does not.

macro require&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

macro require&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> any Error

Check that an expression always throws an error matching some condition, and throw an error if it does not.

Deprecated

