

- Swift
- Bool
-  random() 

Type Method

# random()

Returns a random Boolean value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func random() -> Bool
```

## Return Value

Either `true` or `false`, randomly chosen with equal probability.

## Discussion

This method returns `true` and `false` with equal probability.

```
let flippedHeads = Bool.random()
if flippedHeads {
    print("Heads, you win!")
} else {
    print("Maybe another try?")
}
```

This method is equivalent to calling `Bool.random(using:)`, passing in the system’s default random generator.

## See Also

### Creating a Random Value

static func random&lt;T>(using: inout T) -> Bool

Returns a random Boolean value, using the given generator as a source for randomness.

