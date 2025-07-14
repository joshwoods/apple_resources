

- Accelerate
-  vImageCVImageFormat_SetUserData(\_:\_:\_:) 

Function

# vImageCVImageFormat_SetUserData(\_:\_:\_:)

Sets the user data of a Core Video image format.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageCVImageFormat_SetUserData(
    _ format: vImageCVImageFormat,
    _ userData: UnsafeMutableRawPointer!,
    _ userDataReleaseCallback: ((vImageCVImageFormat?, UnsafeMutableRawPointer?) -> Void)!
) -> vImage_Error
```

## Parameters 

`format`  

The Core Video image format to update.

`userData`  

The new user data for the format.

`userDataReleaseCallback`  

The callback the system calls when it releases the vImageCVImageFormat instance or overwrites the `userData` pointer.

## Return Value

kvImageNoError; otherwise, one of the error codes in Data Types and Constants.

## Discussion

## See Also

### Querying and setting the user data

func vImageCVImageFormat_GetUserData(vImageConstCVImageFormat) -> UnsafeMutableRawPointer!

Returns the user data of a Core Video image format.

