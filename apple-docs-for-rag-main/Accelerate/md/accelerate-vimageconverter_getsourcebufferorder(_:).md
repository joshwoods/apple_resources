

- Accelerate
-  vImageConverter_GetSourceBufferOrder(\_:) 

Function

# vImageConverter_GetSourceBufferOrder(\_:)

Returns a list of vImage source buffer channel names, specifying the order of planes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConverter_GetSourceBufferOrder(_ converter: vImageConverter) -> UnsafePointer!
```

## Parameters 

`converter`  

A valid vImageConverter instance to query the source buffer channel names and order of planes.

## Return Value

An array of buffer type codes (see vImage Buffer Type Codes) that ends with kvImageBufferTypeCode_EndOfList.

## Discussion

This function describes the identity of each buffer passed in the `srcs` parameters of vImageConvert_AnyToAny(_:_:_:_:_:), so you can order the buffers correctly. It’s provided for informational purposes, to help you configure image processing pipelines to vImage that aren’t supported through more direct means.

## See Also

### Querying a converter’s properties

func vImageConverter_MustOperateOutOfPlace(vImageConverter, UnsafePointer&lt;vImage_Buffer>!, UnsafePointer&lt;vImage_Buffer>!, vImage_Flags) -> vImage_Error

Determines whether a converter is capable of operating in place.

func vImageConverter_GetDestinationBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage destination buffer channel names, specifying the order of planes.

func vImageConverter_GetNumberOfSourceBuffers(vImageConverter) -> UInt

Returns the number of source buffers consumed by the converter.

func vImageConverter_GetNumberOfDestinationBuffers(vImageConverter) -> UInt

Returns the number of destination buffers written to by the converter.

