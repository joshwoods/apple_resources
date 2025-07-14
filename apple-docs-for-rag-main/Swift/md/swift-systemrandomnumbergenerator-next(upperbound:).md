

- Swift
- SystemRandomNumberGenerator
-  next(upperBound:) 

Instance Method

# next(upperBound:)

Returns a random value that is less than the given upper bound.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func next(upperBound: T) -> T where T : FixedWidthInteger, T : UnsignedInteger
```

## Parameters 

`upperBound`  

The upper bound for the randomly generated value. Must be non-zero.

## Return Value

A random value of `T` in the range `0..

## Discussion

Use this method when you need random binary data to generate another value. If you need an integer value within a specific range, use the static `random(in:using:)` method on that integer type instead of this method.

## See Also

### Generating Random Binary Data

func next() -> UInt64

Returns a value from a uniform, independent distribution of binary data.

func next&lt;T>() -> T

Returns a value from a uniform, independent distribution of binary data.

