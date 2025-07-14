

- Spatial
- Angle2D
-  ==(\_:\_:) 

Operator

# ==(\_:\_:)

Returns a Boolean value that indicates whether two angles are equal.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func == (lhs: Angle2D, rhs: Angle2D) -> Bool
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## Return Value

A Boolean value that indicates whether two values are equal.

## Discussion

Note

That this operator compares the raw value of each angle and doesn’t normalize the values. For example, 360° doesn’t equal 0°.

