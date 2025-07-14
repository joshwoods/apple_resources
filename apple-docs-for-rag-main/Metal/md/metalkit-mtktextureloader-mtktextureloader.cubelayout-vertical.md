

- MetalKit
- MTKTextureLoader
- MTKTextureLoader.CubeLayout
-  vertical 

Type Property

# vertical

Specifies that the source 2D image is a vertical arrangement of six cube faces.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
static let vertical: MTKTextureLoader.CubeLayout
```

## Discussion

The texture loader creates a cube texture from six faces arranged vertically within a single 2D image. The image height must be six times the image width, with faces arranged in the following order from top to bottom: +X, -X, +Y, -Y, +Z, -Z.

