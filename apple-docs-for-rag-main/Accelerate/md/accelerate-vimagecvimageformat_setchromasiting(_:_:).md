

- Accelerate
-  vImageCVImageFormat_SetChromaSiting(\_:\_:) 

Function

# vImageCVImageFormat_SetChromaSiting(\_:\_:)

Sets the chrominance siting of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_SetChromaSiting(
    _ format: vImageCVImageFormat,
    _ siting: CFString!
) -> vImage_Error
```

## Parameters 

`format`  

The Core Video image format to update.

`siting`  

The new siting information for the format.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

4:2:0 and 4:2:0 YpCbCr image formats that have subsampled chrominance require the position of the chrominance samples relative to the luminance samples.

## See Also

### Related Documentation

var chromaSiting: vImageCVImageFormat.ChromaSiting?

The chrominance siting of the Core Video image format.

### Querying and setting the chrominance siting

func vImageCVImageFormat_GetChromaSiting(vImageConstCVImageFormat) -> Unmanaged&lt;CFString>!

Returns the chrominance siting of a Core Video image format.

