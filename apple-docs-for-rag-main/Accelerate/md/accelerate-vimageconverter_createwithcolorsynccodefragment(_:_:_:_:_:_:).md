

- Accelerate
-  vImageConverter_CreateWithColorSyncCodeFragment(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConverter_CreateWithColorSyncCodeFragment(\_:\_:\_:\_:\_:\_:)

Creates a vImage converter to convert from one vImage Core Graphics image format to another, using custom ColorSync transform.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 7.0+visionOS 1.0+watchOS 1.0+

``` source
func vImageConverter_CreateWithColorSyncCodeFragment(
    _ codeFragment: CFTypeRef,
    _ srcFormat: UnsafePointer,
    _ destFormat: UnsafePointer!,
    _ backgroundColor: UnsafePointer!,
    _ flags: vImage_Flags,
    _ error: UnsafeMutablePointer!
) -> Unmanaged!
```

## Parameters 

`codeFragment`  

A code fragment created with ColorSyncTransformCopyProperty(_:_:_:).

`srcFormat`  

A pointer to a populated vImage_CGImageFormat structure describing the image format of the source image. If the CGColorSpace value is `NULL`, sRGB is used as the default value. The CGColorSpace value is retained by this function and is released when the vImageConverter is destroyed.

`destFormat`  

A pointer to a populated vImage_CGImageFormat structure describing the image format of the destination image. If the CGColorSpace value is `NULL`, sRGB is used as the default value. The CGColorSpace value is retained by this function and is released when the vImageConverter is destroyed.

`backgroundColor`  

An array of floats to be used as a background color if one is needed. The `backgroundColor` range is assumed to be `[0,1]`. The channel ordering and number of color channels must match the natural order of the destination colorspace (for example, RGB or CMYK). The `backgroundColor` value may be `NULL` if no background color is needed.

`flags`  

The options to use when performing this operation. The following flags are supported:

| Name | Description |
|----|----|
| kvImagePrintDiagnosticsToConsole | Prints a debug message if the operation fails. |
| kvImageDoNotTile | Operates as if kvImageDoNotTile was passed to vImageConvert_AnyToAny(_:_:_:_:_:). |

## Return Value

kvImageNoError; otherwise, one of the error codes described in Data Types and Constants.

## Discussion

This function creates a vImageConverter instance to convert between image formats described by vImage_CGImageFormat. The vImageConverter is intended to be used and reused with vImageConvert_AnyToAny(_:_:_:_:_:) to convert images from one format to another.

If `codeFragment` is `NULL`, no colorspace conversion or correction is done. In this case, behavior is undefined if the colorspaces don’t have the same channel order, if they have a different number of channels, or if the colorspaces aren’t from the same family.

kColorSyncTransformFullConversionData is required for black point compensation.

Important

vImageConverter_CreateWithColorSyncCodeFragment(_:_:_:_:_:_:) doesn’t verify that the code fragment is actually appropriate for the source and destination formats provided. Nor does it attempt to append additional color space transformation steps to make sure the code fragment is appropriate to the images provided. If the colorspace of the source and destination formats don’t correspond to the ColorSyncProfile objects used to create the ColorSync transform in the colorspace model, the behavior is undefined.

## See Also

### Creating a converter

class vImageConverter

A description of a conversion from one image format to another.

func vImageConverter_CreateWithCGImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

func vImageConverter_CreateWithCGColorConversionInfo(CGColorConversionInfo, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates an any-to-any converter that uses a color conversion information object to convert from one image format to another.

func vImageConverter_CreateForCGToCVImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, vImageCVImageFormat, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

func vImageConverter_CreateForCVToCGImageFormat(vImageCVImageFormat, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

