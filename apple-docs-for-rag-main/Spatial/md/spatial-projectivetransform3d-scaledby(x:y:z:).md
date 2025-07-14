

- Spatial
- ProjectiveTransform3D
-  scaledBy(x:y:z:) 

Instance Method

# scaledBy(x:y:z:)

Returns a transform that results from scaling with the specified double-precision values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func scaledBy(
    x: Double,
    y: Double,
    z: Double
) -> ProjectiveTransform3D
```

## Parameters 

`x`  

The double-precision value that specifies the scale along the width dimension.

`y`  

The double-precision value that specifies the scale along the height dimension.

`z`  

The double-precision value that specifies the scale along the depth dimension.

## Return Value

The transform that results from scaling with the specified double-precision values.

