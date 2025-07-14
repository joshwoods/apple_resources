

- Metal
- MTLTextureUsage
-  shaderRead 

Type Property

# shaderRead

An option for reading or sampling from the texture in a shader.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var shaderRead: MTLTextureUsage { get }
```

## Discussion

Set this option if you access the given texture with a `read()` or `sample()` function in any shader. This option enables the `access::read` and `access::sample` attributes for the texture. For more information about texture functions and access attributes, see Metal Shading Language Guide.

If the texture is a read-write texture that you also access with a `write()` function in the same shader, set the shaderWrite option to enable the `access::read_write` attribute.

## See Also

### Specifying Texture Usage Options

static var unknown: MTLTextureUsage

An option for a texture whose usage is unknown.

static var shaderWrite: MTLTextureUsage

An option for writing to the texture in a shader.

static var renderTarget: MTLTextureUsage

An option for rendering to the texture in a render pass.

static var pixelFormatView: MTLTextureUsage

An option to create texture views with a different component layout.

