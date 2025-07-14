

- Metal
- MTLTexture
-  parentRelativeSlice 

Instance Property

# parentRelativeSlice

The base slice of the parent texture used to create this texture.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var parentRelativeSlice: Int { get }
```

**Required**

## Discussion

This property is only valid for textures created from a parent texture. The default value is `0`.

## See Also

### Getting Information about Ancestor Resources

var parent: (any MTLTexture)?

The parent texture used to create this texture, if any.

**Required**

var parentRelativeLevel: Int

The base level of the parent texture used to create this texture.

**Required**

var buffer: (any MTLBuffer)?

The source buffer used to create this texture, if any.

**Required**

var bufferOffset: Int

The offset in the source buffer where the texture’s data comes from.

**Required**

var bufferBytesPerRow: Int

The number of bytes in each row of the texture’s source buffer.

**Required**

var rootResource: (any MTLResource)?

The resource that owns the storage for this texture.

**Required**

Deprecated

