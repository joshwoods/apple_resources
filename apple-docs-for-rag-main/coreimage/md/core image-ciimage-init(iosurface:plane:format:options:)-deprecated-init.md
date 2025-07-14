

- Core Image
- CIImage
-  init(ioSurface:plane:format:options:) Deprecated

Initializer

# init(ioSurface:plane:format:options:)

Initializes, using the specified format and options, an image with the contents of a specific data plane in an IOSurface.

macOS 10.9–10.11Deprecated

``` source
init(
    ioSurface surface: IOSurfaceRef,
    plane: Int,
    format: CIFormat,
    options: [CIImageOption : Any]? = nil
)
```

## Parameters 

`surface`  

An IOSurface object.

`plane`  

The index of the data plane in the IOSurface object containing bitmap data for initializing the image.

`format`  

A pixel format constant. See `Pixel Formats`.

`options`  

A dictionary specifying image options. (See `Image Dictionary Keys`.)

## Return Value

An image object initialized with the data from the IOSurface.

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

static let textureTarget: CIImageOption

The key for an OpenGL texture target.

Deprecated

static let textureFormat: CIImageOption

The key for an OpenGL texture format.

Deprecated

