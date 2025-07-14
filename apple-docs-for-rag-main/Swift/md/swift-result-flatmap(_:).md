

- Swift
- Result
-  flatMap(\_:) 

Instance Method

# flatMap(\_:)

Returns a new result, mapping any success value using the given transformation and unwrapping the produced result.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func flatMap(_ transform: (Success) -> Result) -> Result where NewSuccess : ~Copyable
```

Available when `Failure` conforms to `Error`.

## Parameters 

`transform`  

A closure that takes the success value of the instance.

## Return Value

A `Result` instance, either from the closure or the previous `.failure`.

## Discussion

Use this method to avoid a nested result when your transformation produces another `Result` type.

In this example, note the difference in the result of using `map` and `flatMap` with a transformation that returns a result type.

```
func getNextInteger() -> Result {
    .success(4)
}
func getNextAfterInteger(_ n: Int) -> Result {
    .success(n + 1)
}

let result = getNextInteger().map { getNextAfterInteger($0) }
// result == .success(.success(5))

let result = getNextInteger().flatMap { getNextAfterInteger($0) }
// result == .success(5)
```

## See Also

### Transforming a Result

func map&lt;NewSuccess>((Success) -> NewSuccess) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation.

func mapError&lt;NewFailure>((Failure) -> NewFailure) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation.

func flatMapError&lt;NewFailure>((Failure) -> Result&lt;Success, NewFailure>) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation and unwrapping the produced result.

