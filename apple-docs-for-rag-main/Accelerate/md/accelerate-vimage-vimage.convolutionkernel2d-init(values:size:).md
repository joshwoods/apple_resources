

- Accelerate
- vImage
- vImage.ConvolutionKernel2D
-  init(values:size:) 

Initializer

# init(values:size:)

Returns a new convolution kernel structure with the size you specify.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    values: [ComponentType],
    size: vImage.Size
)
```

## Parameters 

`values`  

The kernel weights or structuring element values that must contain `height * width` elements.

`size`  

The size of the kernel. The width and height of the kernel that must be a positive, odd numbers.

## See Also

### Initializers

init(values: [ComponentType], width: Int, height: Int)

Returns a new convolution kernel structure with the width and height you specify.

