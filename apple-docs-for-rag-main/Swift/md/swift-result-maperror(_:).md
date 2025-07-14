

- Swift
- Result
-  mapError(\_:) 

Instance Method

# mapError(\_:)

Returns a new result, mapping any failure value using the given transformation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
consuming func mapError(_ transform: (Failure) -> NewFailure) -> Result where NewFailure : Error
```

Available when `Failure` conforms to `Error`.

## Parameters 

`transform`  

A closure that takes the failure value of the instance.

## Return Value

A `Result` instance with the result of evaluating `transform` as the new failure value if this instance represents a failure.

## Discussion

Use this method when you need to transform the value of a `Result` instance when it represents a failure. The following example transforms the error value of a result by wrapping it in a custom `Error` type:

```
struct DatedError: Error {
    var error: Error
    var date: Date

    init(_ error: Error) {
        self.error = error
        self.date = Date()
    }
}

let result: Result = // ...
// result == .failure()
let resultWithDatedError = result.mapError { DatedError($0) }
// result == .failure(DatedError(error: , date: ))
```

## See Also

### Transforming a Result

func map&lt;NewSuccess>((Success) -> NewSuccess) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation.

func flatMap&lt;NewSuccess>((Success) -> Result&lt;NewSuccess, Failure>) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation and unwrapping the produced result.

func flatMapError&lt;NewFailure>((Failure) -> Result&lt;Success, NewFailure>) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation and unwrapping the produced result.

