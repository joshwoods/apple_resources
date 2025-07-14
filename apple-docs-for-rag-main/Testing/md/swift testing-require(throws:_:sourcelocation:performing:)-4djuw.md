

- Swift Testing
-  require(throws:\_:sourceLocation:performing:) 

Macro

# require(throws:\_:sourceLocation:performing:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@discardableResult @freestanding(expression)
macro require(
    throws error: E,
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation,
    performing expression: () async throws -> R
) -> E where E : Equatable, E : Error
```

## Return Value

The instance of `E` that was thrown by `expression` and is equal to `error`.

## Overview

Throws

An instance of ExpectationFailedError if `expression` does not throw a matching error. The error thrown by `expression` is not rethrown.

Use this overload of `#require()` when the expression `expression` *should* throw a specific error:

```
try #require(throws: EngineFailureError.batteryDied) {
  FoodTruck.shared.engine.batteryLevel = 0
  try FoodTruck.shared.engine.start()
}
```

If `expression` does not throw an error, or if it throws an error that is not equal to `error`, an Issue is recorded for the test that is running in the current task and an instance of ExpectationFailedError is thrown. Any value returned by `expression` is discarded.

If the thrown error need only be an instance of a particular type, use require(throws:_:sourceLocation:performing:) instead.

## See Also

### Checking that errors are thrown

Testing for errors in Swift code

Ensure that your code handles errors in the way you expect.

macro expect&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws an error of a given type.

macro expect&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E?

Check that an expression always throws a specific error.

macro expect&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> (any Error)?

Check that an expression always throws an error matching some condition.

Deprecated

macro require&lt;E, R>(throws: E.Type, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

Check that an expression always throws an error of a given type, and throw an error if it does not.

macro require&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> any Error

Check that an expression always throws an error matching some condition, and throw an error if it does not.

Deprecated

