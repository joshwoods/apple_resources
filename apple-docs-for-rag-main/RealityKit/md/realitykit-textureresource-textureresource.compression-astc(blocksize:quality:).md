

- RealityKit
- TextureResource
- TextureResource.Compression
-  astc(blockSize:quality:) 

Type Method

# astc(blockSize:quality:)

Compresses the imported image with ASTC.

Mac Catalyst 18.0+macOS 15.0+

``` source
static func astc(
    blockSize: TextureResource.Compression.ASTCBlockSize,
    quality: TextureResource.Compression.ASTCQuality = .fast
) -> TextureResource.Compression
```

## Discussion

If the device doesn’t support ASTC pixel formats, RealityKit applies compression as part of the `.reality` file export.

Note

Remove an unused alpha channel from the source image to get better compression quality.

## See Also

### Specifying the compression settings

static var `default`: TextureResource.Compression

A texture you can create and export with lossy compression.

static var none: TextureResource.Compression

A texture you can create with no compression.

enum ASTCBlockSize

The compressed block size.

enum ASTCQuality

Selects the level of processing time allocated to achieve compression.

