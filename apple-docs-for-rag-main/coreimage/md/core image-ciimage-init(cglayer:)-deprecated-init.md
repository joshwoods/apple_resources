

- Core Image
- CIImage
-  init(cgLayer:) Deprecated

Initializer

# init(cgLayer:)

Initializes an image object from the contents supplied by a CGLayer object.

macOS 10.4–10.11Deprecated

``` source
init(cgLayer layer: CGLayer)
```

## Parameters 

`layer`  

A CGLayer object. For more information see Quartz 2D Programming Guide and `CGLayer`.

## Return Value

The initialized image object.

## See Also

### Deprecated

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

static let textureFormat: CIImageOption

The key for an OpenGL texture format.

Deprecated

### Related Documentation

+ imageWithCGLayer:

Creates and returns an image object from the contents supplied by a `CGLayer` object.

