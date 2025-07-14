

- Model I/O
-  MDLMeshBufferType 

Enumeration

# MDLMeshBufferType

Options for the content of a mesh buffer, used by the type property and by MDLMeshBufferAllocator methods for creating buffers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
enum MDLMeshBufferType
```

## Topics

### Constants

case vertex

The buffer contains per-vertex data for one or more vertex attributes of a MDLMesh object.

case index

The buffer contains index data for a MDLSubmesh object.

### Enumeration Cases

case custom

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

