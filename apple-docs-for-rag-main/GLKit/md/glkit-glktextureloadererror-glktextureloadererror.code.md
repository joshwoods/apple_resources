

- GLKit
- GLKTextureLoaderError
-  GLKTextureLoaderError.Code 

Enumeration

# GLKTextureLoaderError.Code

Values to be returned when a texture loader encounters an error.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
enum Code
```

## Topics

### Initializers

init?(rawValue: GLuint)

### Type Properties

case alphaPremultiplicationFailure

The texture source data does not allow the alpha to be premultiplied.

case compressedTextureUpload

A compressed texture could not be uploaded.

case cubeMapInvalidNumFiles

The incorrect number of files were specified for the cube map.

case dataPreprocessingFailure

The data could not be preprocessed correctly.

case fileOrURLNotFound

A file could not be found at the path provided.

case incompatibleFormatSRGB

The decoded data was in an incompatible format for an sRGB texture.

case invalidCGImage

The image provided was invalid.

case invalidEAGLContext

The EAGL context was not a valid context.

case invalidNSData

The data provided is not in a recognized image format.

case mipmapUnsupported

The texture source data does not allow mipmaps to be generated.

case pvrAtlasUnsupported

Cube maps may not be compressed in PVRTC format.

case reorientationFailure

The texture source data does not allow the image to be reoriented.

case uncompressedTextureUpload

An uncompressed texture could not be uploaded.

case unknownFileType

The file was in an unrecognized format.

case unknownPathType

The path type was unrecognized.

case unsupportedBitDepth

The data in the source image has an unsupported bit depth.

case unsupportedCubeMapDimensions

The cube map’s dimensions are incorrect.

case unsupportedOrientation

The texture source data is stored with an unsupported origin position.

case unsupportedPVRFormat

The data in the PVRTC compressed format is in an unsupported format.

case unsupportedTextureTarget

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

typealias GLKTextureLoaderCallback

Signature for the block executed after an asynchronous texture loading operation completes.

Texture Loading Options

Keys to specify in a `textureOperations` dictionary.

Texture Error Handling

Strings used when handling error messages returned from a texture loading method.

