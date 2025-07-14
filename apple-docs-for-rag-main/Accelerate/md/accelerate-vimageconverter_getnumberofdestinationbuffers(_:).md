

- Accelerate
-  vImageConverter_GetNumberOfDestinationBuffers(\_:) 

Function

# vImageConverter_GetNumberOfDestinationBuffers(\_:)

Returns the number of destination buffers written to by the converter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConverter_GetNumberOfDestinationBuffers(_ converter: vImageConverter) -> UInt
```

## Parameters 

`converter`  

A valid converter to query the number of source buffers.

## Return Value

The number of destination buffers.

## Discussion

This function is for video formats that are planar data formats with data in more than one plane.

## See Also

### Querying a converter’s properties

func vImageConverter_MustOperateOutOfPlace(vImageConverter, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Determines whether a converter is capable of operating in place.

func vImageConverter_GetSourceBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage source buffer channel names, specifying the order of planes.

func vImageConverter_GetDestinationBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage destination buffer channel names, specifying the order of planes.

func vImageConverter_GetNumberOfSourceBuffers(vImageConverter) -> UInt

Returns the number of source buffers consumed by the converter.

