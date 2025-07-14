

- Accelerate
- vImage_PerpsectiveTransform
-  init(source:destination:) 

Initializer

# init(source:destination:)

Returns a projective-transformation structure that defines the mapping between a source quadrilateral and a destination quadrilateral.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
init?(
    source: vImage_PerpsectiveTransform.QuadrilateralPoints,
    destination: vImage_PerpsectiveTransform.QuadrilateralPoints
)
```

## Parameters 

`source`  

The four source points.

`destination`  

The four destination points.

## See Also

### Creating a projective-transformation structure

init()

Creates a projective-transformation structure.

init(a: Float, b: Float, c: Float, d: Float, tx: Float, ty: Float, vx: Float, vy: Float, v: Float)

Creates a projective-transformation structure from the specified single-precision values.

