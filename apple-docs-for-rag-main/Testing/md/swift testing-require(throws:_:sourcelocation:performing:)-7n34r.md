

- Swift Testing
-  require(throws:\_:sourceLocation:performing:) 

Macro

# require(throws:\_:sourceLocation:performing:)

Check that an expression always throws an error of a given type, and throw an error if it does not.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSSwift 6.0+Xcode 16.0+

``` source
@discardableResult @freestanding(expression)
macro require(
    throws errorType: E.Type,
    _ comment: @autoclosure () -> Comment? = nil,
    sourceLocation: SourceLocation = #_sourceLocation,
    performing expression: () async throws -> R
) -> E where E : Error
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

The instance of `errorType` that was thrown by `expression`.

## Overview

Throws

An instance of ExpectationFailedError if `expression` does not throw a matching error. The error thrown by `expression` is not rethrown.

Use this overload of `#require()` when the expression `expression` *should* throw an error of a given type:

```
try #require(throws: EngineFailureError.self) {
  FoodTruck.shared.engine.batteryLevel = 0
  try FoodTruck.shared.engine.start()
}
```

If `expression` does not throw an error, or if it throws an error that is not an instance of `errorType`, an Issue is recorded for the test that is running in the current task and an instance of ExpectationFailedError is thrown. Any value returned by `expression` is discarded.

If the thrown error need only equal another instance of Error, use require(throws:_:sourceLocation:performing:) instead.

If `expression` should *never* throw, simply invoke the code without using this macro. The test will then fail if an error is thrown.

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

macro require&lt;E, R>(throws: E, @autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R) -> E

macro require&lt;R>(@autoclosure () -> Comment?, sourceLocation: SourceLocation, performing: () async throws -> R, throws: (any Error) async throws -> Bool) -> any Error

Check that an expression always throws an error matching some condition, and throw an error if it does not.

Deprecated

