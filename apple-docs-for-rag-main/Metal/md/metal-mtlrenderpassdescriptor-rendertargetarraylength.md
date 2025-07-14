

- Metal
- MTLRenderPassDescriptor
-  renderTargetArrayLength 

Instance Property

# renderTargetArrayLength

The number of active layers that all attachments must have for layered rendering.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.11+tvOS 14.5+visionOS 1.0+

``` source
var renderTargetArrayLength: Int { get set }
```

## Mentioned in 

Rendering to Multiple Texture Slices in a Draw Command

## Discussion

The default value is `0`, indicating that the GPU does not use layered rendering on this render pass.

The table below gives typical values you might set, depending on the type of texture being used as attachments in the render pass. Your vertex shader must select the render target array index between `0` and the array length minus `1`.

| Texture Type | Typical Length |
|----|----|
| MTLTextureType.type1DArray or MTLTextureType.type2DArray | The length of the texture array (arrayLength) |
| MTLTextureType.typeCube | 6 |
| MTLTextureType.typeCubeArray | 6 times the length of the texture array (arrayLength) |

## See Also

### Layered Rendering

var renderTargetWidth: Int

The width, in pixels, to constrain the render target to.

var renderTargetHeight: Int

The height, in pixels, to constrain the render target to.

