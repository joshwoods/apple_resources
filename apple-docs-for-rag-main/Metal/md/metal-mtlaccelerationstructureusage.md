

- Metal
-  MTLAccelerationStructureUsage 

Structure

# MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
struct MTLAccelerationStructureUsage
```

## Topics

### Creating Usage Options

init(rawValue: UInt)

Creates new usage options from a raw integer value.

### Usage Options

static var refit: MTLAccelerationStructureUsage

An option that specifies that you can refit the acceleration structure if the geometry changes.

static var preferFastBuild: MTLAccelerationStructureUsage

An option that specifies that Metal needs to build the acceleration structure quickly, even if that reduces ray-tracing performance.

static var extendedLimits: MTLAccelerationStructureUsage

A structure usage option that indicates you intend to use larger ray-tracing limits for the acceleration structure.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Acceleration Structures

Improving Ray-Tracing Data Access Using Per-Primitive Data

Simplify data access and improve GPU utilization by storing custom primitive data directly in the acceleration structure.

protocol MTLAccelerationStructure

A collection of model data for GPU-accelerated intersection of rays with the model.

class MTLAccelerationStructureDescriptor

A base class for classes that define the configuration for a new acceleration structure.

class MTLPrimitiveAccelerationStructureDescriptor

A description of an acceleration structure that contains geometry primitives.

class MTLInstanceAccelerationStructureDescriptor

A description of an acceleration structure that derives from instances of primitive acceleration structures.

protocol MTLAccelerationStructureCommandEncoder

An object for encoding commands that build or refit acceleration structures.

struct MTLAccelerationStructureRefitOptions

