

- Accelerate
-  vImageCVImageFormat_GetUserData(\_:) 

Function

# vImageCVImageFormat_GetUserData(\_:)

Returns the user data of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_GetUserData(_ format: vImageConstCVImageFormat) -> UnsafeMutableRawPointer!
```

## Parameters 

`format`  

The Core Video image format to query.

## Return Value

The address of `userData;` `NULL` if `userData` isn’t set.

## Discussion

The functions that create Core Video image formats, such as vImageCVImageFormat_CreateWithCVPixelBuffer(_:), return a vImageCVImageFormat. The following code shows how you create a vImageConstCVImageFormat representation of a vImageCVImageFormat instance to pass to vImageCVImageFormat_GetUserData(_:):

```
let userData = withUnsafeBytes(of: cvImageFormat) { bytes in
    let format = bytes.assumingMemoryBound(
        to: vImageConstCVImageFormat.self).first!

    return vImageCVImageFormat_GetUserData(format)
}
```

## See Also

### Querying and setting the user data

func vImageCVImageFormat_SetUserData(vImageCVImageFormat, UnsafeMutableRawPointer!, ((vImageCVImageFormat?, UnsafeMutableRawPointer?) -> Void)!) -> vImage_Error

Sets the user data of a Core Video image format.

