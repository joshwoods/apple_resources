

- Metal
- MTLTexture
-  iosurfacePlane 

Instance Property

# iosurfacePlane

The number of a plane within the underlying surface instance for the texture, if applicable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.11+tvOS 11.0+visionOS 1.0+

``` source
var iosurfacePlane: Int { get }
```

**Required**

## Discussion

The plane number applies to the iosurfacePlane property when it isn’t `nil`. The property’s value defaults to `0` for textures that don’t come from an IOSurface instance.

## See Also

### Getting Information about the IOSurface the Texture Was Created From

var iosurface: IOSurfaceRef?

A reference to the underlying surface instance for the texture, if applicable.

**Required**

