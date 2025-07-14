

- Metal
- MTLTextureUsage
-  unknown 

Type Property

# unknown

An option for a texture whose usage is unknown.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var unknown: MTLTextureUsage { get }
```

## Mentioned in 

Optimizing Texture Data

## Discussion

Set this option if you’re not sure how your app uses the given texture, but you want to be able to use it in many ways. This might be the case if you have multiple code paths and it’s unclear how your app specifically uses the texture at runtime.

This is the most flexible usage option for a texture, but it incurs a significant performance cost. Metal can’t optimize operations for the texture if you don’t set specific usage options.

In iOS devices with GPU family 5, Metal doesn’t apply lossless compression to the given texture if you set this option.

## See Also

### Specifying Texture Usage Options

static var shaderRead: MTLTextureUsage

An option for reading or sampling from the texture in a shader.

static var shaderWrite: MTLTextureUsage

An option for writing to the texture in a shader.

static var renderTarget: MTLTextureUsage

An option for rendering to the texture in a render pass.

static var pixelFormatView: MTLTextureUsage

An option to create texture views with a different component layout.

