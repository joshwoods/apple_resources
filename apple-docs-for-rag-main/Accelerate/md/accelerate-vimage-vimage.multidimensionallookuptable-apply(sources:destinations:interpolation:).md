

- Accelerate
- vImage
- vImage.MultidimensionalLookupTable
-  apply(sources:destinations:interpolation:) 

Instance Method

# apply(sources:destinations:interpolation:)

Transforms an array of planar pixel buffers using the multidimensional lookup table.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func apply(
    sources: [vImage.PixelBuffer],
    destinations: [vImage.PixelBuffer],
    interpolation: vImage.MultidimensionalLookupTable.InterpolationMethod
)
```

## Parameters 

`sources`  

An array that contains sourceChannelCount vImage.PlanarF buffers.

`destinations`  

An array that contains destinationChannelCount vImage.PlanarF buffers.

`interpolation`  

An enumeration that specifies how the operation computes output color values that don’t have an explicit entry in the table.

## See Also

### Instance Methods

func apply&lt;SrcFormat, DestFormat>(source: vImage.PixelBuffer&lt;SrcFormat>, destination: vImage.PixelBuffer&lt;DestFormat>, interpolation: vImage.MultidimensionalLookupTable.InterpolationMethod)

Transforms a multiple plane pixel buffer using the multidimensional lookup table.

