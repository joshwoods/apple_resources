

- Metal
- MTLBuffer
-  makeRemoteBufferView(\_:) 

Instance Method

# makeRemoteBufferView(\_:)

Creates a remote view of the buffer for another GPU in the same peer group.

macOS 10.15+

``` source
func makeRemoteBufferView(_ device: any MTLDevice) -> (any MTLBuffer)?
```

**Required**

## Mentioned in 

Transferring Data Between Connected GPUs

## Discussion

The device object that created this buffer, and the device object passed into this method, must have the same nonzero peer group identifier (peerGroupID). This buffer must use the private storage mode (MTLStorageMode.private).

A remote view doesn’t allocate any storage for the new buffer; it references the memory allocated for the original buffer. You can use remote views only as a source for copy commands encoded by a MTLBlitCommandEncoder. For more information, see Transferring Data Between Connected GPUs.

## See Also

### Creating Views of Buffers on Other GPUs

var remoteStorageBuffer: (any MTLBuffer)?

The buffer on another GPU that the buffer was created from, if any.

**Required**

