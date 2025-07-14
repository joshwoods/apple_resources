

- Swift
- Result
-  flatMapError(\_:) 

Instance Method

# flatMapError(\_:)

Returns a new result, mapping any failure value using the given transformation and unwrapping the produced result.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
consuming func flatMapError(_ transform: (Failure) -> Result) -> Result where NewFailure : Error
```

Available when `Failure` conforms to `Error`.

## Parameters 

`transform`  

A closure that takes the failure value of the instance.

## Return Value

A `Result` instance, either from the closure or the previous `.success`.

## See Also

### Transforming a Result

func map&lt;NewSuccess>((Success) -> NewSuccess) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation.

func mapError&lt;NewFailure>((Failure) -> NewFailure) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation.

func flatMap&lt;NewSuccess>((Success) -> Result&lt;NewSuccess, Failure>) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation and unwrapping the produced result.

