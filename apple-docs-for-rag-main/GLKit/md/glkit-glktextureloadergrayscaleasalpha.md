

- GLKit
-  GLKTextureLoaderGrayscaleAsAlpha 

Global Variable

# GLKTextureLoaderGrayscaleAsAlpha

Whether or not to treat greyscale image data as alpha information.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
let GLKTextureLoaderGrayscaleAsAlpha: String
```

## Discussion

This key specifies whether the image data in a grayscale image should be treated as alpha information. The value for this key is an NSNumber object that specifies a boolean value. If false, the image data is treated as luminance data. If true, the image data is treated as alpha data. The default value is false. This key is ignored if the source image is not a grayscale image.

## See Also

### Constants

let GLKTextureLoaderApplyPremultiplication: String

Whether image data should be premultiplied before being loaded into the sharegroup.

let GLKTextureLoaderErrorDomain: String

The error domain used by GLKit when returning texture loading errors.

Deprecated

let GLKTextureLoaderErrorKey: String

A key used to retrieve an error string from an error object userinfo dictionary.

Deprecated

let GLKTextureLoaderGLErrorKey: String

A key used to retrieve additional information from an error object’s userinfo dictionary.

Deprecated

let GLKTextureLoaderGenerateMipmaps: String

Whether or not to create mipmaps for a texture.

let GLKTextureLoaderOriginBottomLeft: String

Whether or not to vertically flip image data to match OpenGL’s coordinate system.

let GLKTextureLoaderSRGB: String

Whether or not to treat texture image data as sRGB data.

Deprecated

var GLK_SSE3_INTRINSICS: Int32

let kGLKModelErrorDomain: StringDeprecated

let kGLKModelErrorKey: StringDeprecated

