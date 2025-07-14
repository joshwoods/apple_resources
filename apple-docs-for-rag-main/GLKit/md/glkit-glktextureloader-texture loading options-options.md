

- GLKit
- GLKTextureLoader
-  Texture Loading Options 

API Collection

# Texture Loading Options

Keys to specify in a `textureOperations` dictionary.

## Topics

### Constants

let GLKTextureLoaderApplyPremultiplication: String

Whether image data should be premultiplied before being loaded into the sharegroup.

let GLKTextureLoaderGenerateMipmaps: String

Whether or not to create mipmaps for a texture.

let GLKTextureLoaderOriginBottomLeft: String

Whether or not to vertically flip image data to match OpenGL’s coordinate system.

let GLKTextureLoaderGrayscaleAsAlpha: String

Whether or not to treat greyscale image data as alpha information.

let GLKTextureLoaderSRGB: String

Whether or not to treat texture image data as sRGB data.

Deprecated

## See Also

### Constants

typealias GLKTextureLoaderCallback

Signature for the block executed after an asynchronous texture loading operation completes.

Texture Error Handling

Strings used when handling error messages returned from a texture loading method.

enum Code

Values to be returned when a texture loader encounters an error.

