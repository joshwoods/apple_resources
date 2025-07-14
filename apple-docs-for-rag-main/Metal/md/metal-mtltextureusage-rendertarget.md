

- Metal
- MTLTextureUsage
-  renderTarget 

Type Property

# renderTarget

An option for rendering to the texture in a render pass.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var renderTarget: MTLTextureUsage { get }
```

## Mentioned in 

Developing Metal apps that run in Simulator

Optimizing Texture Data

## Discussion

Set this option if you use the given texture as a color, depth, or stencil render target in any render pass. This option allows you to assign the texture to the texture property of a MTLRenderPassAttachmentDescriptor.

Important

Rendering and writing to a texture are different operations, and you don’t need to combine their usage options. Set the renderTarget option if you render to a given texture, but don’t set the shaderWrite option if you don’t write to the texture. The renderTarget and shaderWrite options aren’t equivalent, and setting renderTarget doesn’t require you to also set shaderWrite.

## See Also

### Specifying Texture Usage Options

static var unknown: MTLTextureUsage

An option for a texture whose usage is unknown.

static var shaderRead: MTLTextureUsage

An option for reading or sampling from the texture in a shader.

static var shaderWrite: MTLTextureUsage

An option for writing to the texture in a shader.

static var pixelFormatView: MTLTextureUsage

An option to create texture views with a different component layout.

