

- Accelerate
- vImage
- vImage.PixelBuffer
-  makeArray(of:channelCount:) 

Instance Method

# makeArray(of:channelCount:)

Returns an array of `width * height * channelCount` values that’s a copy of the buffer’s visible contents.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func makeArray(
    of scalarType: U.Type,
    channelCount: Int
) -> [U]
```

Available when `Format` is `vImage.DynamicPixelFormat`.

## Parameters 

`scalarType`  

The scalar type of each array element.

`channelCount`  

The number of channels in the pixel buffer.

## Return Value

An array of `scalarType` values that contains the source buffer’s contents.

