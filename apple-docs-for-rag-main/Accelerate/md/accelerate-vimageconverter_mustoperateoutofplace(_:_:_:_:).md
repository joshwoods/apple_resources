

- Accelerate
-  vImageConverter_MustOperateOutOfPlace(\_:\_:\_:\_:) 

Function

# vImageConverter_MustOperateOutOfPlace(\_:\_:\_:\_:)

Determines whether a converter is capable of operating in place.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConverter_MustOperateOutOfPlace(
    _ converter: vImageConverter,
    _ srcs: UnsafePointer!,
    _ dests: UnsafePointer!,
    _ flags: vImage_Flags
) -> vImage_Error
```

## Parameters 

`converter`  

The converter to check to determine if it’s capable of operating in place.

`srcs`  

The list of source buffers you plan to use with vImageConvert_AnyToAny(_:_:_:_:_:). This parameter may be `NULL`.

`dests`  

The list of destination buffers you plan to use with vImageConvert_AnyToAny(_:_:_:_:_:). This parameter may be `NULL`.

`flags`  

The flags you’ll pass to vImageConvert_AnyToAny(_:_:_:_:_:).

## Return Value

kvImageNoError if the conversion will work in place, kvImageOutOfPlaceOperationRequired if the conversion requires out of place operation; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

Some conversions work if the source and destination image buffer scanlines start at the same address. Others don’t; for those cases, you need to allocate additional storage to hold the destination buffer.

In-place operation is considered to mean `srcs[i].data = dests[i].data` and `srcs[i].rowBytes = dests[i].rowBytes`. Other styles of partial buffer overlap produce undefined behavior.

## See Also

### Querying a converter’s properties

func vImageConverter_GetSourceBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage source buffer channel names, specifying the order of planes.

func vImageConverter_GetDestinationBufferOrder(vImageConverter) -> UnsafePointer&lt;vImageBufferTypeCode>!

Returns a list of vImage destination buffer channel names, specifying the order of planes.

func vImageConverter_GetNumberOfSourceBuffers(vImageConverter) -> UInt

Returns the number of source buffers consumed by the converter.

func vImageConverter_GetNumberOfDestinationBuffers(vImageConverter) -> UInt

Returns the number of destination buffers written to by the converter.

