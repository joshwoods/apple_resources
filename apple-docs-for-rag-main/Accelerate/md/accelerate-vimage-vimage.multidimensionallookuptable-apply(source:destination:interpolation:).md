

- Accelerate
- vImage
- vImage.MultidimensionalLookupTable
-  apply(source:destination:interpolation:) 

Instance Method

# apply(source:destination:interpolation:)

Transforms a multiple plane pixel buffer using the multidimensional lookup table.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func apply(
    source: vImage.PixelBuffer,
    destination: vImage.PixelBuffer,
    interpolation: vImage.MultidimensionalLookupTable.InterpolationMethod
) where SrcFormat : MultiplePlanePixelFormat, DestFormat : MultiplePlanePixelFormat, SrcFormat.ComponentType == Float, DestFormat.ComponentType == Float
```

## Parameters 

`source`  

A multiple plane Pixel_F pixel buffer that contains sourceChannelCount planes.

`destination`  

A multiple plane Pixel_F pixel buffer that contains destinationChannelCount planes.

`interpolation`  

An enumeration that specifies how the operation computes output color values that don’t have an explicit entry in the table.

## See Also

### Instance Methods

func apply(sources: [vImage.PixelBuffer&lt;vImage.PlanarF>], destinations: [vImage.PixelBuffer&lt;vImage.PlanarF>], interpolation: vImage.MultidimensionalLookupTable.InterpolationMethod)

Transforms an array of planar pixel buffers using the multidimensional lookup table.

