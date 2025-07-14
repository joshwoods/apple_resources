

- Core Image
- CIImage
- CIImageOption
-  textureFormat Deprecated

Type Property

# textureFormat

The key for an OpenGL texture format.

macOS 10.9–10.14Deprecated

``` source
static let textureFormat: CIImageOption
```

## Discussion

The value for this key must be an NSNumber object containing a Core Image pixel format constant. (See `Pixel Formats`.) You may only use this key when initializing an image using the init(texture:size:flipped:options:) method.

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

init(texture: UInt32, size: CGSize, flipped: Bool, options: [CIImageOption : Any]?)

Initializes an image object with data supplied by an OpenGL texture.

Deprecated

init(ioSurface: IOSurfaceRef, plane: Int, format: CIFormat, options: [CIImageOption : Any]?)

Initializes, using the specified format and options, an image with the contents of a specific data plane in an IOSurface.

Deprecated

static let textureTarget: CIImageOption

The key for an OpenGL texture target.

Deprecated

