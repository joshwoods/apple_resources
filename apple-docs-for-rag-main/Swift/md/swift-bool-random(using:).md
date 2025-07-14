

- Swift
- Bool
-  random(using:) 

Type Method

# random(using:)

Returns a random Boolean value, using the given generator as a source for randomness.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func random(using generator: inout T) -> Bool where T : RandomNumberGenerator
```

## Parameters 

`generator`  

The random number generator to use when creating the new random value.

## Return Value

Either `true` or `false`, randomly chosen with equal probability.

## Discussion

This method returns `true` and `false` with equal probability. Use this method to generate a random Boolean value when you are using a custom random number generator.

```
let flippedHeads = Bool.random(using: &myGenerator)
if flippedHeads {
    print("Heads, you win!")
} else {
    print("Maybe another try?")
}
```

Note

The algorithm used to create random values may change in a future version of Swift. If you’re passing a generator that results in the same sequence of Boolean values each time you run your program, that sequence may change when your program is compiled using a different version of Swift.

## See Also

### Creating a Random Value

static func random() -> Bool

Returns a random Boolean value.

