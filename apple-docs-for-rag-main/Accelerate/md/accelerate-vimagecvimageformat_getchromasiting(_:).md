

- Accelerate
-  vImageCVImageFormat_GetChromaSiting(\_:) 

Function

# vImageCVImageFormat_GetChromaSiting(\_:)

Returns the chrominance siting of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetChromaSiting(_ format: vImageConstCVImageFormat) -> Unmanaged!
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

A CFString that describes the positioning of the chrominance samples.

## Discussion

4:2:0 and 4:2:0 YpCbCr image formats that have subsampled chrominance require the position of the chrominance samples relative to the luminance samples.

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetChromaSiting(_:):

```
let chromaSiting = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetChromaSiting(format)
}
```

## See Also

### Related Documentation

var chromaSiting: vImageCVImageFormat.ChromaSiting?

The chrominance siting of the Core Video image format.

### Querying and setting the chrominance siting

func vImageCVImageFormat_SetChromaSiting(vImageCVImageFormat, CFString!) -> vImage_Error

Sets the chrominance siting of a Core Video image format.

