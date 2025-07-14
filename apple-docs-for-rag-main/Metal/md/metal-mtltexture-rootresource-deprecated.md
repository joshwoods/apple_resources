

- Metal
- MTLTexture
-  rootResource Deprecated

Instance Property

# rootResource

The resource that owns the storage for this texture.

iOS 8.0–10.0DeprecatediPadOS 8.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.12DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var rootResource: (any MTLResource)? { get }
```

**Required**

Deprecated

Use parent or buffer instead.

## Discussion

If the value is `nil`, then this texture image owns its own data. Otherwise, this value is the MTLResource instance used to create the texture. For example, it might be a texture that uses the contents of an MTLBuffer object or a texture view that reinterprets the contents of another MTLTexture.

## See Also

### Getting Information about Ancestor Resources

var parent: (any MTLTexture)?

The parent texture used to create this texture, if any.

**Required**

var parentRelativeLevel: Int

The base level of the parent texture used to create this texture.

**Required**

var parentRelativeSlice: Int

The base slice of the parent texture used to create this texture.

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

