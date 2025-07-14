

- GLKit
-  GLKTextureLoaderSRGB Deprecated

Global Variable

# GLKTextureLoaderSRGB

Whether or not to treat texture image data as sRGB data.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0DeprecatedmacOS 10.9–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
let GLKTextureLoaderSRGB: String
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Discussion

The value for this key is an NSNumber object that specifies a boolean value. If false, the image data is treated as linear pixel data. If true, the image data is treated as sRGB pixel data. The default value is false.

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

let GLKTextureLoaderGrayscaleAsAlpha: String

Whether or not to treat greyscale image data as alpha information.

let GLKTextureLoaderOriginBottomLeft: String

Whether or not to vertically flip image data to match OpenGL’s coordinate system.

var GLK_SSE3_INTRINSICS: Int32

let kGLKModelErrorDomain: StringDeprecated

let kGLKModelErrorKey: StringDeprecated

