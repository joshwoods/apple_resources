

- GLKit
-  GLKMesh Deprecated

Class

# GLKMesh

iOS 9.0–12.0DeprecatediPadOS 9.0–12.0DeprecatedmacOS 10.11–10.14DeprecatedtvOS 9.0–12.0Deprecated

``` source
class GLKMesh
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Topics

### Initializers

init(mesh: MDLMesh) throws

### Instance Properties

var name: String

var submeshes: [GLKSubmesh]

var vertexBuffers: [GLKMeshBuffer]

var vertexCount: Int

var vertexDescriptor: MDLVertexDescriptor

### Type Methods

class func newMeshes(from: MDLAsset, sourceMeshes: AutoreleasingUnsafeMutablePointer&lt;NSArray?>?) throws -> [GLKMesh]

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Mesh Data Management

class GLKMeshBufferDeprecated

class GLKMeshBufferAllocatorDeprecated

class GLKSubmeshDeprecated

