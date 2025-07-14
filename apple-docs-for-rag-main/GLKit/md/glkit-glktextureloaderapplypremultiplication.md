

- GLKit
-  GLKTextureLoaderApplyPremultiplication 

Global Variable

# GLKTextureLoaderApplyPremultiplication

Whether image data should be premultiplied before being loaded into the sharegroup.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0–12.0Deprecated

``` source
let GLKTextureLoaderApplyPremultiplication: String
```

## Discussion

The value for this key is an NSNumber object that specifies a boolean value. If false, the data is loaded into the sharegroup without being modified. If true, the red, green and blue components of each pixel are multiplied by the alpha value. If the key is not specified, the default value is false. Never specify true for a texture that is in a compressed format.

## See Also

### Constants

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

let GLKTextureLoaderSRGB: String

Whether or not to treat texture image data as sRGB data.

Deprecated

var GLK_SSE3_INTRINSICS: Int32

let kGLKModelErrorDomain: StringDeprecated

let kGLKModelErrorKey: StringDeprecated

