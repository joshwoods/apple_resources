

- Core Image
- CIImage
-  init(texture:size:flipped:options:) Deprecated

Initializer

# init(texture:size:flipped:options:)

Initializes an image object with data supplied by an OpenGL texture.

macOS 10.9–10.14Deprecated

``` source
init(
    texture name: UInt32,
    size: CGSize,
    flipped: Bool,
    options: [CIImageOption : Any]? = nil
)
```

## Parameters 

`name`  

An OpenGL texture. Because `CIImage` objects are immutable, the texture must remain unchanged for the life of the image object. See the discussion for more information.

`size`  

The dimensions of the texture.

`flag`  

`true` to have Core Image flip the coordinates of the texture vertically to convert between OpenGL and Core Image coordinate systems.

`options`  

A dictionary specifying image options. (See `Image Dictionary Keys`.)

## Return Value

The initialized image object.

## Discussion

When using a texture to create a `CIImage` object, the texture must be valid in the Core Image context (CIContext) that you draw the `CIImage` object into. This means that one of the following must be true:

- The texture must be created using the `CGLContext` object that the CIContext is based on.

- The context that the texture was created in must be shared with the `CGLContext` that the CIContextis based on.

Note that textures do not have a retain and release mechanism. This means that your application must make sure that the texture exists for the life cycle of the image. When you no longer need the image, you can delete the texture.

Core Image ignores the texture filtering and wrap modes (`GL_TEXTURE_FILTER` and `GL_TEXTURE_WRAP`) that you set through OpenGL. The filter and wrap modes are overridden by what the CISampler object specifies when you apply a filter to the `CIImage` object.

## See Also

### Deprecated

init(cgLayer: CGLayer)

Initializes an image object from the contents supplied by a CGLayer object.

Deprecated

init(cgLayer: CGLayer, options: [CIImageOption : Any]?)

Initializes an image object from the contents supplied by a CGLayer object, using the specified options.

Deprecated

init(texture: UInt32, size: CGSize, flipped: Bool, colorSpace: CGColorSpace?)

Initializes an image object with data supplied by an OpenGL texture.

Deprecated

init(ioSurface: IOSurfaceRef, plane: Int, format: CIFormat, options: [CIImageOption : Any]?)

Initializes, using the specified format and options, an image with the contents of a specific data plane in an IOSurface.

Deprecated

static let textureTarget: CIImageOption

The key for an OpenGL texture target.

Deprecated

static let textureFormat: CIImageOption

The key for an OpenGL texture format.

Deprecated

### Related Documentation

+ imageWithTexture:size:flipped:options:

Creates and returns an image object initialized with data supplied by an OpenGL texture.

