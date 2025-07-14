

- GameplayKit
-  GKQuad 

Structure

# GKQuad

The definition of an axis-aligned rectangle addressed by the tree.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
struct GKQuad
```

## Topics

### Initializers

init()

init(quadMin: vector_float2, quadMax: vector_float2)

### Instance Properties

var quadMax: vector_float2

The corner of the rectangle with the highest coordinate values (in most coordinate systems, the upper-right corner).

var quadMin: vector_float2

The corner of the rectangle with the lowest coordinate values (in most coordinate systems, the lower-left corner).

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

