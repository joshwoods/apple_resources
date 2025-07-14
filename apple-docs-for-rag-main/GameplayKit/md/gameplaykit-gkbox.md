

- GameplayKit
-  GKBox 

Structure

# GKBox

The definition of an axis-aligned rectangular bounding volume addressed by the tree.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct GKBox
```

## Topics

### Initializers

init()

init(boxMin: vector_float3, boxMax: vector_float3)

### Instance Properties

var boxMax: vector_float3

The corner of the box with the highest coordinate values (in most coordinate systems, the near-upper-right corner).

var boxMin: vector_float3

The corner of the box with the lowest coordinate values (in most coordinate systems, the far-lower-left corner).

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

