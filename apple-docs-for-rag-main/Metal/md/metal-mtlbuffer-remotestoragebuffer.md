

- Metal
- MTLBuffer
-  remoteStorageBuffer 

Instance Property

# remoteStorageBuffer

The buffer on another GPU that the buffer was created from, if any.

macOS 10.15+

``` source
var remoteStorageBuffer: (any MTLBuffer)? { get }
```

**Required**

## Discussion

If the value of this property is non-`nil`, it contains a reference to the MTLBuffer object that created this buffer. If the buffer isn’t a remote view, the value of this property is `nil`.

You can use remote views only as a source for copy commands encoded by a MTLBlitCommandEncoder.

## See Also

### Creating Views of Buffers on Other GPUs

func makeRemoteBufferView(any MTLDevice) -> (any MTLBuffer)?

Creates a remote view of the buffer for another GPU in the same peer group.

**Required**

