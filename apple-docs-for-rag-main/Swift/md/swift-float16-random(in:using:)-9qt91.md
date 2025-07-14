

- Swift
- Float16
-  random(in:using:) 

Type Method

# random(in:using:)

Returns a random value within the specified range, using the given generator as a source for randomness.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func random(
    in range: Range,
    using generator: inout T
) -> Self where T : RandomNumberGenerator
```

Available when `RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`range`  

The range in which to create a random value. `range` must be finite and non-empty.

`generator`  

The random number generator to use when creating the new random value.

## Return Value

A random value within the bounds of `range`.

## Discussion

Use this method to generate a floating-point value within a specific range when you are using a custom random number generator. This example creates three new values in the range `10.0 ..

```
for _ in 1...3 {
    print(Double.random(in: 10.0 ..

The `random(in:using:)` static method chooses a random value from a continuous uniform distribution in `range`, and then converts that value to the nearest representable value in this type. Depending on the size and span of `range`, some concrete values may be represented more frequently than others.

Note

The algorithm used to create random values may change in a future version of Swift. If you’re passing a generator that results in the same sequence of floating-point values each time you run your program, that sequence may change when your program is compiled using a different version of Swift.

