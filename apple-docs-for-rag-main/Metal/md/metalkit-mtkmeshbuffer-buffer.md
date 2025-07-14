

- MetalKit
- MTKMeshBuffer
-  buffer 

Instance Property

# buffer

The Metal buffer backing all vertex and index data.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var buffer: any MTLBuffer { get }
```

## Discussion

Many MTKMeshBuffer objects may reference the same MTLBuffer object, in which case each MTKMeshBuffer object will have its own unique offset value.

## See Also

### Metal Buffer Properties

var length: Int

The logical size of the Metal buffer, in bytes.

var offset: Int

The byte offset of the data within the Metal buffer.

