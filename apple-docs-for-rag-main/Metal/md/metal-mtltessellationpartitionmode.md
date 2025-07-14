

- Metal
-  MTLTessellationPartitionMode 

Enumeration

# MTLTessellationPartitionMode

Options for choosing the partition mode that the tessellator applies when deriving the number and spacing of segments for subdividing a corresponding edge.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
enum MTLTessellationPartitionMode
```

## Overview

The table lists the tessellation factor range for each partitioning mode.

| Partitioning mode | Tessellation factor range |
|----|----|
| MTLTessellationPartitionMode.pow2 | \[`1`, maxTessellationFactor\] |
| MTLTessellationPartitionMode.integer | \[`1`, maxTessellationFactor\] |
| MTLTessellationPartitionMode.fractionalOdd | \[`1`, maxTessellationFactor-1\] |
| MTLTessellationPartitionMode.fractionalEven | \[`2`, maxTessellationFactor\] |

The floating-point tessellation level is always clamped to its corresponding range before calculating the final tessellation factor. After clamping, the calculation depends on the chosen partitioning mode:

- For the MTLTessellationPartitionMode.pow2 partitioning mode, the result is rounded up to the nearest integer `n`, where `n` is a power of two. The corresponding edge is divided into `n` segments of equal length in (u, v) space.

- For the MTLTessellationPartitionMode.integer partitioning mode, the result is rounded up to the nearest integer `n`. The corresponding edge is divided into `n` segments of equal length in (u, v) space.

- For the MTLTessellationPartitionMode.fractionalOdd partitioning mode, the tessellation level is rounded up the the nearest odd integer `n`. If `n` is `1`, the edge is not subdivided. Otherwise, the corresponding edge is divided into `n-2` segments of equal length, and two additional segments of equal length that are typically shorter than the other segments. The length of the two additional segments relative to the others decreases monotonically by the value of `n-f`, where `f` is the clamped floating-point tessellation level. If `n-f` is `0` the additional segments equal length to the other segments. As `n-f` approaches `2`, the relative length of the additional segments approaches `0`. The two additional segments should be placed symmetrically on opposite sides of the subdivided edge. The relative location of these two segments is undefined, but must be identical for any pair of subdivided edges with identical values of `f`.

- For the MTLTessellationPartitionMode.fractionalEven partitioning mode, the tessellation level is rounded up the the nearest even integer `n`.

## Topics

### Constants

case pow2

A power of two partitioning mode.

case integer

An integer partitioning mode.

case fractionalOdd

A fractional odd partitioning mode.

case fractionalEven

A fractional even partitioning mode.

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

### Specifying Tessellation State

var maxTessellationFactor: Int

The maximum tessellation factor that the tessellator uses when tessellating patches.

var isTessellationFactorScaleEnabled: Bool

A Boolean value that determines whether the pipeline scales the tessellation factor.

var tessellationFactorFormat: MTLTessellationFactorFormat

The format of the tessellation factors in the tessellation factor buffer.

var tessellationControlPointIndexType: MTLTessellationControlPointIndexType

The size of the control point indices in a control point index buffer.

var tessellationFactorStepFunction: MTLTessellationFactorStepFunction

The step function for determining the tessellation factors for a patch from the tessellation factor buffer.

var tessellationOutputWindingOrder: MTLWinding

The winding order of triangles from the tessellator.

var tessellationPartitionMode: MTLTessellationPartitionMode

The partitioning mode that the tessellator uses to derive the number and spacing of segments for subdividing a corresponding edge.

enum MTLTessellationFactorFormat

Options for specifying the format of the tessellation factors in a tessellation factor buffer.

enum MTLTessellationControlPointIndexType

Options for specifying the size of the control point indices in a control point index buffer.

enum MTLTessellationFactorStepFunction

Options for specifying the step function that determines the tessellation factors for a patch from the tessellation factor buffer.

