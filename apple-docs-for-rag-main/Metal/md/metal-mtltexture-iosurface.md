

- Metal
- MTLTexture
-  iosurface 

Instance Property

# iosurface

A reference to the underlying surface instance for the texture, if applicable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.11+tvOS 11.0+visionOS 1.0+

``` source
var iosurface: IOSurfaceRef? { get }
```

**Required**

## Discussion

The property’s value is `nil` for textures that don’t come from an IOSurface instance.

## See Also

### Getting Information about the IOSurface the Texture Was Created From

var iosurfacePlane: Int

The number of a plane within the underlying surface instance for the texture, if applicable.

**Required**

