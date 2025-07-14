

- Swift
- SystemRandomNumberGenerator
-  next() 

Instance Method

# next()

Returns a value from a uniform, independent distribution of binary data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func next() -> T where T : FixedWidthInteger, T : UnsignedInteger
```

## Return Value

A random value of `T`. Bits are randomly distributed so that every value of `T` is equally likely to be returned.

## Discussion

Use this method when you need random binary data to generate another value. If you need an integer value within a specific range, use the static `random(in:using:)` method on that integer type instead of this method.

## See Also

### Generating Random Binary Data

func next() -> UInt64

Returns a value from a uniform, independent distribution of binary data.

func next&lt;T>(upperBound: T) -> T

Returns a random value that is less than the given upper bound.

