

- Group Activities
- SpatialTemplateElementDirection
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Adds the y-axis rotations for the specified values together and returns a new structure with the result.

visionOS 2.0+

``` source
static func + (lhs: SpatialTemplateElementDirection, rhs: Angle2D) -> SpatialTemplateElementDirection
```

## Parameters 

`lhs`  

The first direction.

`rhs`  

The second direction.

## Return Value

A new direction type that combines the rotations from `lhs` and `rhs`.

