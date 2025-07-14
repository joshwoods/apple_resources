

- Metal
- MTLTextureUsage
-  shaderWrite 

Type Property

# shaderWrite

An option for writing to the texture in a shader.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var shaderWrite: MTLTextureUsage { get }
```

## Mentioned in 

Optimizing Texture Data

## Discussion

Set this option if you access the given texture with a `write()` function in any shader. This option enables the `access::write` attribute for the texture. For more information about texture functions and access attributes, see Metal Shading Language Guide.

If the texture is a read-write texture that you also access with a `read()` function in the same shader, set the shaderRead option to enable the `access::read_write` attribute.

In iOS devices with GPU family 5, Metal doesn’t apply lossless compression to the given texture if you set this option.

Important

Rendering and writing to a texture are different operations, and you don’t need to combine their usage options. Set the renderTarget option if you render to a given texture, but don’t set the shaderWrite option if you don’t write to the texture. The renderTarget and shaderWrite options aren’t equivalent, and setting renderTarget doesn’t require you to also set shaderWrite.

## See Also

### Specifying Texture Usage Options

static var unknown: MTLTextureUsage

An option for a texture whose usage is unknown.

static var shaderRead: MTLTextureUsage

An option for reading or sampling from the texture in a shader.

static var renderTarget: MTLTextureUsage

An option for rendering to the texture in a render pass.

static var pixelFormatView: MTLTextureUsage

An option to create texture views with a different component layout.

