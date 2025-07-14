

- Swift
-  Result 

Enumeration

# Result

A value that represents either a success or a failure, including an associated value in each case.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
enum Result where Failure : Error, Success : ~Copyable
```

## Mentioned in 

Preserving the Results of a Throwing Expression

Writing Failable Asynchronous APIs

## Topics

### Representing a Result

case success(Success)

A success, storing a `Success` value.

case failure(Failure)

A failure, storing a `Failure` value.

Writing Failable Asynchronous APIs

Vend results as part of an API when you can’t return errors synchronously.

### Converting a Throwing Expression to a Result

Preserving the Results of a Throwing Expression

Call the initializer that wraps a throwing expression when you need to serialize or memoize the result.

init(catching: () throws(Failure) -> Success)

Creates a new result by evaluating a throwing closure, capturing the returned value as a success, or any thrown error as a failure.

### Converting a Result to a Throwing Expression

func get() throws(Failure) -> Success

Returns the success value as a throwing expression.

### Transforming a Result

func map&lt;NewSuccess>((Success) -> NewSuccess) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation.

func mapError&lt;NewFailure>((Failure) -> NewFailure) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation.

func flatMap&lt;NewSuccess>((Success) -> Result&lt;NewSuccess, Failure>) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation and unwrapping the produced result.

func flatMapError&lt;NewFailure>((Failure) -> Result&lt;Success, NewFailure>) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation and unwrapping the produced result.

### Comparing Results

static func == (Result&lt;Success, Failure>, Result&lt;Success, Failure>) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Publishing a Result

var publisher: Result&lt;Success, Failure>.Publisher

A Combine publisher that publishes this instance’s result to each subscriber exactly once, or fails immediately if the result indicates failure.

struct Publisher

The type of a Combine publisher that publishes this instance’s result to each subscriber exactly once, or fails immediately if the result indicates failure.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Success` conforms to `Copyable`, `Success` conforms to `Escapable`, and `Failure` conforms to `Error`.

- Equatable

  Conforms when `Success` conforms to `Hashable`, `Failure` conforms to `Error`, and `Failure` conforms to `Hashable`.

- Hashable

  Conforms when `Success` conforms to `Hashable`, `Failure` conforms to `Error`, and `Failure` conforms to `Hashable`.

- Sendable

  Conforms when `Success` conforms to `Escapable`, `Success` conforms to `Sendable`, and `Failure` conforms to `Error`.

## See Also

### Errors

protocol Error

A type representing an error value that can be thrown.

