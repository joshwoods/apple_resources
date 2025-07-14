

- Accelerate
- vImage
- vImage.ConvolutionKernel2D
-  width 

Instance Property

# width

The width of the kernel that must be a positive, odd number.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
let width: vImagePixelCount
```

## See Also

### Instance Properties

let height: vImagePixelCount

The height of the kernel that must be a positive, odd number.

let values: [ComponentType]

The kernel weights or structuring element values that must contain `height * width` elements.

