

- Swift
- Result
-  init(catching:) 

Initializer

# init(catching:)

Creates a new result by evaluating a throwing closure, capturing the returned value as a success, or any thrown error as a failure.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(catching body: () throws(Failure) -> Success)
```

Available when `Failure` conforms to `Error`.

## Parameters 

`body`  

A potentially throwing closure to evaluate.

## Mentioned in 

Preserving the Results of a Throwing Expression

## See Also

### Converting a Throwing Expression to a Result

Preserving the Results of a Throwing Expression

Call the initializer that wraps a throwing expression when you need to serialize or memoize the result.

