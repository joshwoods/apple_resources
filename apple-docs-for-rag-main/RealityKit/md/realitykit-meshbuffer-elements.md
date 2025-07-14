

- RealityKit
- MeshBuffer
-  elements 

Instance Property

# elements

Access the buffer as an array. This may create a copy if the data are not already an array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var elements: [Element] { get }
```

## See Also

### Inspecting a mesh

let count: Int

The number of elements in the buffer.

typealias Element

A type representing the sequence’s elements.

var rate: MeshBuffers.Rate

Rate of the buffer.

