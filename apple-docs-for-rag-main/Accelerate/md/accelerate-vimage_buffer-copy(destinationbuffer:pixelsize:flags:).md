

- Accelerate
- vImage_Buffer
-  copy(destinationBuffer:pixelSize:flags:) 

Instance Method

# copy(destinationBuffer:pixelSize:flags:)

Copies the contents of a vImage buffer to the specified destination buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func copy(
    destinationBuffer: inout vImage_Buffer,
    pixelSize: Int,
    flags options: vImage.Options = .noFlags
) throws
```

## Parameters 

`destinationBuffer`  

The destination buffer.

`pixelSize`  

The number of bytes for one pixel.

`options`  

The options to use when performing the operation.

