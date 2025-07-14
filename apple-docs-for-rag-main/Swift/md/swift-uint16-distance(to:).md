

- Swift
- UInt16
-  distance(to:) 

Instance Method

# distance(to:)

Returns the distance from this value to the given value, expressed as a stride.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func distance(to other: Self) -> Int
```

## Parameters 

`other`  

The value to calculate the distance to.

## Return Value

The distance from this value to `other`.

## Discussion

For two values `x` and `y`, and a distance `n = x.distance(to: y)`, `x.advanced(by: n) == y`.

