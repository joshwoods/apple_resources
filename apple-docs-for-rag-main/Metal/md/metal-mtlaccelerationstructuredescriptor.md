

- Metal
-  MTLAccelerationStructureDescriptor 

Class

# MTLAccelerationStructureDescriptor

A base class for classes that define the configuration for a new acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLAccelerationStructureDescriptor
```

## Overview

This is the base class for other acceleration structure descriptors. Don’t use this class directly. Use one of the derived classes instead, as MTLAccelerationStructure describes.

## Topics

### Specifying Usage Options

var usage: MTLAccelerationStructureUsage

The options that describe how you intend to use the acceleration structure.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MTLIndirectInstanceAccelerationStructureDescriptor
- MTLInstanceAccelerationStructureDescriptor
- MTLPrimitiveAccelerationStructureDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Acceleration Structures

Improving Ray-Tracing Data Access Using Per-Primitive Data

Simplify data access and improve GPU utilization by storing custom primitive data directly in the acceleration structure.

protocol MTLAccelerationStructure

A collection of model data for GPU-accelerated intersection of rays with the model.

class MTLPrimitiveAccelerationStructureDescriptor

A description of an acceleration structure that contains geometry primitives.

class MTLInstanceAccelerationStructureDescriptor

A description of an acceleration structure that derives from instances of primitive acceleration structures.

protocol MTLAccelerationStructureCommandEncoder

An object for encoding commands that build or refit acceleration structures.

struct MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

struct MTLAccelerationStructureRefitOptions

