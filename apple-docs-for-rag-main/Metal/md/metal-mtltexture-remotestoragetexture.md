

- Metal
- MTLTexture
-  remoteStorageTexture 

Instance Property

# remoteStorageTexture

The texture on another GPU that the texture was created from, if any.

macOS 10.15+

``` source
var remoteStorageTexture: (any MTLTexture)? { get }
```

**Required**

## Discussion

If the value of this property is non-`nil`, it contains a reference to the MTLTexture object that created this texture. If the texture isn’t a remote view, the value of this property is `nil`.

You can use remote views only as the source for copy commands encoded by a MTLBlitCommandEncoder.

## See Also

### Creating Views of Textures on Other GPUs

func makeRemoteTextureView(any MTLDevice) -> (any MTLTexture)?

Creates a remote texture view for another GPU in the same peer group.

**Required**

