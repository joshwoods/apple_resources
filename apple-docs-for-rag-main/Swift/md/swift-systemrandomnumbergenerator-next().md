

- Swift
- SystemRandomNumberGenerator
-  next() 

Instance Method

# next()

Returns a value from a uniform, independent distribution of binary data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func next() -> UInt64
```

## Return Value

An unsigned 64-bit random value.

## See Also

### Generating Random Binary Data

func next&lt;T>() -> T

Returns a value from a uniform, independent distribution of binary data.

func next&lt;T>(upperBound: T) -> T

Returns a random value that is less than the given upper bound.

