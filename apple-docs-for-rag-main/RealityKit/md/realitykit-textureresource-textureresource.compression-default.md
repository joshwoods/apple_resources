

- RealityKit
- TextureResource
- TextureResource.Compression
-  default 

Type Property

# default

A texture you can create and export with lossy compression.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
static var `default`: TextureResource.Compression { get }
```

## Discussion

The selected compression preserves perceptual texture details (no aggressive compression).

## See Also

### Specifying the compression settings

static var none: TextureResource.Compression

A texture you can create with no compression.

static func astc(blockSize: TextureResource.Compression.ASTCBlockSize, quality: TextureResource.Compression.ASTCQuality) -> TextureResource.Compression

Compresses the imported image with ASTC.

enum ASTCBlockSize

The compressed block size.

enum ASTCQuality

Selects the level of processing time allocated to achieve compression.

