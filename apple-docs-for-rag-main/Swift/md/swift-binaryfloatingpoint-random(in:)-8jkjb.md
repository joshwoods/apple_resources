

- Swift
- BinaryFloatingPoint
-  random(in:) 

Type Method

# random(in:)

Returns a random value within the specified range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static func random(in range: Range) -> Self
```

Available when `RawSignificand` conforms to `FixedWidthInteger`.

## Parameters 

`range`  

The range in which to create a random value. `range` must be finite and non-empty.

## Return Value

A random value within the bounds of `range`.

## Discussion

Use this method to generate a floating-point value within a specific range. This example creates three new values in the range `10.0 ..

```
for _ in 1...3 {
    print(Double.random(in: 10.0 ..

The `random()` static method chooses a random value from a continuous uniform distribution in `range`, and then converts that value to the nearest representable value in this type. Depending on the size and span of `range`, some concrete values may be represented more frequently than others.

This method is equivalent to calling `random(in:using:)`, passing in the system’s default random generator.

## See Also

### Creating a Random Value

static func random(in: ClosedRange&lt;Self>) -> Self

Returns a random value within the specified range.

static func random&lt;T>(in: ClosedRange&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

static func random&lt;T>(in: Range&lt;Self>, using: inout T) -> Self

Returns a random value within the specified range, using the given generator as a source for randomness.

