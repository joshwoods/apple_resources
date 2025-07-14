

- Swift
- Optional
-  flatMap(\_:) 

Instance Method

# flatMap(\_:)

Evaluates the given closure when this `Optional` instance is not `nil`, passing the unwrapped value as a parameter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func flatMap(_ transform: (Wrapped) throws(E) -> U?) throws(E) -> U? where E : Error, U : ~Copyable
```

## Parameters 

`transform`  

A closure that takes the unwrapped value of the instance.

## Return Value

The result of the given closure. If this instance is `nil`, returns `nil`.

## Discussion

Use the `flatMap` method with a closure that returns an optional value. This example performs an arithmetic operation with an optional result on an optional integer.

```
let possibleNumber: Int? = Int("42")
let nonOverflowingSquare = possibleNumber.flatMap { x -> Int? in
    let (result, overflowed) = x.multipliedReportingOverflow(by: x)
    return overflowed ? nil : result
}
print(nonOverflowingSquare)
// Prints "Optional(1764)"
```

## See Also

### Transforming an Optional Value

func map&lt;E, U>((Wrapped) throws(E) -> U) throws(E) -> U?

Evaluates the given closure when this `Optional` instance is not `nil`, passing the unwrapped value as a parameter.

