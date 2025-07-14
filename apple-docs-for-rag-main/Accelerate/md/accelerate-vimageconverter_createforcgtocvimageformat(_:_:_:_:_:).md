

- Accelerate
-  vImageConverter_CreateForCGToCVImageFormat(\_:\_:\_:\_:\_:) 

Function

# vImageConverter_CreateForCGToCVImageFormat(\_:\_:\_:\_:\_:)

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 8.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConverter_CreateForCGToCVImageFormat(
    _ srcFormat: UnsafePointer,
    _ destFormat: vImageCVImageFormat,
    _ backgroundColor: UnsafePointer!,
    _ flags: vImage_Flags,
    _ error: UnsafeMutablePointer!
) -> Unmanaged!
```

## Parameters 

`srcFormat`  

The vImage_CGImageFormat structure that describes the pixel format associated with the source buffers.

`destFormat`  

The vImageCVImageFormat structure that describes the pixel format associated with the destination image buffers.

`backgroundColor`  

In cases where the source format has an alpha channel and the destination doesn’t (or is CGImageAlphaInfo.noneSkipFirst or CGImageAlphaInfo.noneSkipLast) the conversion removes the alpha channel by flattening it against an opaque background color. The background color is specified as three CGFloat values corresponding to red, green, and blue in sRGB.

`flags`  

The options to use when performing this operation. The following flags are supported:

| Name | Description |
|----|----|
| kvImagePrintDiagnosticsToConsole | Prints a debug message if the operation fails. |
| kvImageHighQualityResampling | Instructs the converter to spend extra time to achieve better image quality in cases where chroma is upsampled or downsampled as part of the conversion. |
| kvImageDoNotTile | Operates as if kvImageDoNotTile was passed to vImageConvert_AnyToAny(_:_:_:_:_:). |

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

This function creates a vImageConverter instance that’s used with vImageConvert_AnyToAny(_:_:_:_:_:) to convert a Core Graphics formatted image, described by vImage_CGImageFormat, to Core Video image data, described by vImageCVImageFormat.

## See Also

### Creating a converter

class vImageConverter

A description of a conversion from one image format to another.

func vImageConverter_CreateWithCGImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

func vImageConverter_CreateWithCGColorConversionInfo(CGColorConversionInfo, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates an any-to-any converter that uses a color conversion information object to convert from one image format to another.

func vImageConverter_CreateForCVToCGImageFormat(vImageCVImageFormat, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

func vImageConverter_CreateWithColorSyncCodeFragment(CFTypeRef, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>!, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter to convert from one vImage Core Graphics image format to another, using custom ColorSync transform.

