

- RealityKit
- MeshBuffer
-  MeshBuffer.Element 

Type Alias

# MeshBuffer.Element

A type representing the sequence’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias Element = Element
```

## See Also

### Inspecting a mesh

let count: Int

The number of elements in the buffer.

var elements: [Element]

Access the buffer as an array. This may create a copy if the data are not already an array.

var rate: MeshBuffers.Rate

Rate of the buffer.

