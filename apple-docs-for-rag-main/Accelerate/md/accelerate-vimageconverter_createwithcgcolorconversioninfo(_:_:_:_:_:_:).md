

- Accelerate
-  vImageConverter_CreateWithCGColorConversionInfo(\_:\_:\_:\_:\_:\_:) 

Function

# vImageConverter_CreateWithCGColorConversionInfo(\_:\_:\_:\_:\_:\_:)

Creates an any-to-any converter that uses a color conversion information object to convert from one image format to another.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func vImageConverter_CreateWithCGColorConversionInfo(
    _ colorConversionInfoRef: CGColorConversionInfo,
    _ sFormat: UnsafePointer,
    _ dFormat: UnsafePointer,
    _ bg: UnsafePointer!,
    _ flags: vImage_Flags,
    _ error: UnsafeMutablePointer!
) -> Unmanaged!
```

## Parameters 

`colorConversionInfoRef`  

The object that describes how to convert between color spaces.

`sFormat`  

A pointer to a populated vImage_CGImageFormat that describes the image format of the source image.

`dFormat`  

A pointer to a populated vImage_CGImageFormat that describes the image format of the destination image.

`bg`  

An array of single-precision values, in the range 0 to 1, that specifies the background color when required.

`flags`  

The options to use when performing this operation.

`error`  

An optional `inout` value that receives an error code.

## Discussion

Use vImageConverter_CreateWithCGColorConversionInfo(_:_:_:_:_:_:) to create a converter suitable for use with vImageConvert_AnyToAny(_:_:_:_:_:), which uses CGColorConversionInfo for color conversion. CGColorConversionInfo provides greater control on the color-space conversion than, for example, using a converter returned by vImageConverter_CreateWithCGImageFormat(_:_:_:_:_:).

### Convert Linear Color Space to sRGB

You can use vImageConverter_CreateWithCGColorConversionInfo(_:_:_:_:_:_:) to convert an image with a linear response curve to sRGB. Many vImage operations provide optimal results when working on images with a linear response curve, this approach is ideal for converting between linear and sRGB.

Begin by creating the source and destination color spaces, and the CGColorConversionInfo instance:

```
guard
    let sourceColorSpace = CGColorSpace(name: CGColorSpace.linearSRGB),
    let destinationColorSpace = CGColorSpace(name: CGColorSpace.sRGB),
    let conversionInfo = CGColorConversionInfo(src: sourceColorSpace,
                                               dst: destinationColorSpace)
else {
    return
}
```

Create a vImage_CGImageFormat structure, without a color space, that specifies the pixel memory requirement, number of channels, and alpha information:

```
var cgImageFormat = vImage_CGImageFormat(bitsPerComponent: 8,
                                         bitsPerPixel: 8 * 3,
                                         colorSpace: nil,
                                         bitmapInfo: CGBitmapInfo(rawValue: CGImageAlphaInfo.none.rawValue),
                                         version: 0,
                                         decode: nil,
                                         renderingIntent: .defaultIntent)
```

Create the converter and buffers:

```
guard
    let converter = vImageConverter_CreateWithCGColorConversionInfo(conversionInfo,
                                                                    &cgImageFormat,
                                                                    &cgImageFormat,
                                                                    [0],
                                                                    vImage_Flags(kvImageNoFlags),
                                                                    nil),
    var sourceBuffer = try? vImage_Buffer(cgImage: sourceCGImage,
                                          format: cgImageFormat),
    var destinationBuffer = try? vImage_Buffer(width: Int(image.size.width),
                                               height: Int(image.size.height),
                                               bitsPerPixel: cgImageFormat.bitsPerPixel) else {
    return
}
```

Pass the converter and the two buffers to vImageConvert_AnyToAny(_:_:_:_:_:) to perform the conversion:

```
vImageConvert_AnyToAny(converter.takeRetainedValue(),
                       &sourceBuffer, &destinationBuffer,
                       nil,
                       vImage_Flags(kvImageNoFlags))
```

The following image shows the source image, on the left, and the contents of `destinationBuffer`, on the right, after conversion:

## See Also

### Creating a converter

class vImageConverter

A description of a conversion from one image format to another.

func vImageConverter_CreateWithCGImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts from one vImage Core Graphics image format to another.

func vImageConverter_CreateForCGToCVImageFormat(UnsafePointer&lt;vImage_CGImageFormat>, vImageCVImageFormat, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Graphics-formatted image to a Core Video-formatted image.

func vImageConverter_CreateForCVToCGImageFormat(vImageCVImageFormat, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter that converts a Core Video-formatted image to a Core Graphics-formatted image.

func vImageConverter_CreateWithColorSyncCodeFragment(CFTypeRef, UnsafePointer&lt;vImage_CGImageFormat>, UnsafePointer&lt;vImage_CGImageFormat>!, UnsafePointer&lt;CGFloat>!, vImage_Flags, UnsafeMutablePointer&lt;vImage_Error>!) -> Unmanaged&lt;vImageConverter>!

Creates a vImage converter to convert from one vImage Core Graphics image format to another, using custom ColorSync transform.

