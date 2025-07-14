

- Swift
- Int
-  Int.Magnitude 

Type Alias

# Int.Magnitude

A type that can represent the absolute value of any possible value of this type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias Magnitude = UInt
```

## See Also

### Finding the Sign and Magnitude

var magnitude: UInt

The magnitude of this value.

func abs&lt;T>(T) -> T

Returns the absolute value of the given number.

func signum() -> Int

Returns `-1` if this value is negative and `1` if it’s positive; otherwise, `0`.

