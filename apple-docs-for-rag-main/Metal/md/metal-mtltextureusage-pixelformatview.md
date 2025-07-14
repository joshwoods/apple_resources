

- Metal
- MTLTextureUsage
-  pixelFormatView 

Type Property

# pixelFormatView

An option to create texture views with a different component layout.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var pixelFormatView: MTLTextureUsage { get }
```

## Mentioned in 

Optimizing Texture Data

## Discussion

Set this option if you need to call any of these methods of the texture to create a texture view with a different component layout:

- makeTextureView(pixelFormat:)

- makeTextureView(pixelFormat:textureType:levels:slices:)

- newTextureViewWithPixelFormat:textureType:levels:slices:

- makeTextureView(pixelFormat:textureType:levels:slices:swizzle:)

- newTextureViewWithPixelFormat:textureType:levels:slices:swizzle:

For example, if your texture uses the MTLPixelFormat.rgba8Unorm pixel format, you can reinterpret the data as MTLPixelFormat.r32Uint. The pixel layout is considered different if the number of components differs, or if their size or order is different from the components in the original pixel format.

Don’t set this option if your texture view needs to read the component values in a different order. Instead, create a texture view with a swizzle pattern that specifies the new order.

Don’t set this option if your texture view only converts between linear space and sRGB. For example, if your texture uses the MTLPixelFormat.rgba8Unorm pixel format and your texture view uses MTLPixelFormat.bgra8Unorm_srgb.

In iOS devices with GPU family 5 and later, Metal doesn’t apply lossless compression to the given texture if you set this option.

## See Also

### Specifying Texture Usage Options

static var unknown: MTLTextureUsage

An option for a texture whose usage is unknown.

static var shaderRead: MTLTextureUsage

An option for reading or sampling from the texture in a shader.

static var shaderWrite: MTLTextureUsage

An option for writing to the texture in a shader.

static var renderTarget: MTLTextureUsage

An option for rendering to the texture in a render pass.

