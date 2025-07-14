

- Vision
-  VNComputeStage 

Structure

# VNComputeStage

Types that represent the compute stage.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct VNComputeStage
```

## Topics

### Get the Compute Stages

static let main: VNComputeStage

A stage that represents where the system performs the main functionality.

static let postProcessing: VNComputeStage

A stage that represents where the system performs additional analysis from the main compute stage.

### Create a Compute Stage

init(rawValue: String)

Creates a compute stage with the value you specify.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Utilities

class VNGeometryUtils

Utility methods to determine the geometries of various Vision types.

class VNVideoProcessor

An object that performs offline analysis of video content.

