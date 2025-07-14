

- Metal
- MTLTexture
-  makeRemoteTextureView(\_:) 

Instance Method

# makeRemoteTextureView(\_:)

Creates a remote texture view for another GPU in the same peer group.

macOS 10.15+

``` source
func makeRemoteTextureView(_ device: any MTLDevice) -> (any MTLTexture)?
```

**Required**

## Mentioned in 

Transferring Data Between Connected GPUs

## Discussion

The device object that created this texture, and the device object passed into this method, must have the same nonzero peer group identifier (peerGroupID). This texture must either use the private storage mode (MTLStorageMode.private) or be backed by an IOSurface.

A remote view doesn’t allocate any storage for the new texture; it references the memory allocated for the original texture. You can use remote views only as a source for copy commands encoded by a MTLBlitCommandEncoder. For more information, see Transferring Data Between Connected GPUs.

## See Also

### Creating Views of Textures on Other GPUs

var remoteStorageTexture: (any MTLTexture)?

The texture on another GPU that the texture was created from, if any.

**Required**

