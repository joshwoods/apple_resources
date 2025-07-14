

- Swift
- Optional
-  map(\_:) 

Instance Method

# map(\_:)

Evaluates the given closure when this `Optional` instance is not `nil`, passing the unwrapped value as a parameter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func map(_ transform: (Wrapped) throws(E) -> U) throws(E) -> U? where E : Error, U : ~Copyable
```

## Parameters 

`transform`  

A closure that takes the unwrapped value of the instance.

## Return Value

The result of the given closure. If this instance is `nil`, returns `nil`.

## Discussion

Use the `map` method with a closure that returns a non-optional value. This example performs an arithmetic operation on an optional integer.

```
let possibleNumber: Int? = Int("42")
let possibleSquare = possibleNumber.map { $0 * $0 }
print(possibleSquare)
// Prints "Optional(1764)"

let noNumber: Int? = nil
let noSquare = noNumber.map { $0 * $0 }
print(noSquare)
// Prints "nil"
```

## See Also

### Transforming an Optional Value

func flatMap&lt;E, U>((Wrapped) throws(E) -> U?) throws(E) -> U?

Evaluates the given closure when this `Optional` instance is not `nil`, passing the unwrapped value as a parameter.

