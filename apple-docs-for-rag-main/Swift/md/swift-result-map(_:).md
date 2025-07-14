

- Swift
- Result
-  map(\_:) 

Instance Method

# map(\_:)

Returns a new result, mapping any success value using the given transformation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func map(_ transform: (Success) -> NewSuccess) -> Result where NewSuccess : ~Copyable
```

Available when `Failure` conforms to `Error`.

## Parameters 

`transform`  

A closure that takes the success value of this instance.

## Return Value

A `Result` instance with the result of evaluating `transform` as the new success value if this instance represents a success.

## Discussion

Use this method when you need to transform the value of a `Result` instance when it represents a success. The following example transforms the integer success value of a result into a string:

```
func getNextInteger() -> Result { /* ... */ }

let integerResult = getNextInteger()
// integerResult == .success(5)
let stringResult = integerResult.map { String($0) }
// stringResult == .success("5")
```

## See Also

### Transforming a Result

func mapError&lt;NewFailure>((Failure) -> NewFailure) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation.

func flatMap&lt;NewSuccess>((Success) -> Result&lt;NewSuccess, Failure>) -> Result&lt;NewSuccess, Failure>

Returns a new result, mapping any success value using the given transformation and unwrapping the produced result.

func flatMapError&lt;NewFailure>((Failure) -> Result&lt;Success, NewFailure>) -> Result&lt;Success, NewFailure>

Returns a new result, mapping any failure value using the given transformation and unwrapping the produced result.

