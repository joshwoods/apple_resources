

- Metal
-  MTLAccelerationStructureRefitOptions 

Structure

# MTLAccelerationStructureRefitOptions

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct MTLAccelerationStructureRefitOptions
```

## Topics

### Initializers

init(rawValue: UInt)

### Type Properties

static var perPrimitiveData: MTLAccelerationStructureRefitOptions

static var vertexData: MTLAccelerationStructureRefitOptions

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

struct MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

