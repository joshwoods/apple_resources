

- Accelerate
- vImage
- vImage.ConvolutionKernel2D
-  init(values:width:height:) 

Initializer

# init(values:width:height:)

Returns a new convolution kernel structure with the width and height you specify.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    values: [ComponentType],
    width: Int,
    height: Int
)
```

## Parameters 

`values`  

The kernel weights or structuring element values that must contain `height * width` elements.

`width`  

The width of the kernel that must be a positive, odd number.

`height`  

The height of the kernel that must be a positive, odd number.

## See Also

### Initializers

init(values: [ComponentType], size: vImage.Size)

Returns a new convolution kernel structure with the size you specify.

