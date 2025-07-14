

- Swift
- UInt32
-  advanced(by:) 

Instance Method

# advanced(by:)

Returns a value that is offset the specified distance from this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func advanced(by n: Int) -> Self
```

## Parameters 

`n`  

The distance to advance this value.

## Return Value

A value that is offset from this value by `n`.

## Discussion

Use the `advanced(by:)` method in generic code to offset a value by a specified distance. If you’re working directly with numeric values, use the addition operator (`+`) instead of this method.

For a value `x`, a distance `n`, and a value `y = x.advanced(by: n)`, `x.distance(to: y) == n`.

