

- Metal
-  MTLPatchType 

Enumeration

# MTLPatchType

Types of tessellation patches that can be inputs of a post-tessellation vertex function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
enum MTLPatchType
```

## Topics

### Patch types

case none

An option that indicates that this isn’t a post-tessellation vertex function.

case triangle

A triangle patch.

case quad

A quad patch.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying the Tessellation Patch

var patchType: MTLPatchType

The tessellation patch type of a post-tessellation vertex function.

**Required**

var patchControlPointCount: Int

The number of patch control points in the post-tessellation vertex function.

**Required**

