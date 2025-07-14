

- RealityKit
- TextureResource
- TextureResource.Compression
-  none 

Type Property

# none

A texture you can create with no compression.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static var none: TextureResource.Compression { get }
```

## Discussion

If you export this to a `.reality` file using write(to:), the texture remains uncompressed.

## See Also

### Specifying the compression settings

static var `default`: TextureResource.Compression

A texture you can create and export with lossy compression.

static func astc(blockSize: TextureResource.Compression.ASTCBlockSize, quality: TextureResource.Compression.ASTCQuality) -> TextureResource.Compression

Compresses the imported image with ASTC.

enum ASTCBlockSize

The compressed block size.

enum ASTCQuality

Selects the level of processing time allocated to achieve compression.

