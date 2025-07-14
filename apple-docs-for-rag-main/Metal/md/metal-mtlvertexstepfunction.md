

- Metal
-  MTLVertexStepFunction 

Enumeration

# MTLVertexStepFunction

The frequency with which the vertex function or post-tessellation vertex function fetches attribute data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLVertexStepFunction
```

## Topics

### Constants

case constant

The vertex function fetches attribute data once and uses that data for every vertex.

case perVertex

The vertex function fetches and uses new attribute data for every vertex.

case perInstance

The vertex function regularly fetches new attribute data for a number of instances that is determined by `stepRate`.

case perPatch

The post-tessellation vertex function fetches data based on the patch index of the patch.

case perPatchControlPoint

The post-tessellation vertex function fetches data based on the control-point indices associated with the patch.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

