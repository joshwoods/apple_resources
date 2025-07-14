

- Metal
-  MTLResidencySetDescriptor 

Class

# MTLResidencySetDescriptor

A configuration that customizes the behavior for a residency set.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
class MTLResidencySetDescriptor
```

## Mentioned in 

Simplifying GPU Resource Management with Residency Sets

## Overview

Make an MTLResidencySet by creating and configuring an MTLResidencySetDescriptor instance and pass it to the makeResidencySet(descriptor:) method of an MTLDevice instance.

See Simplifying GPU Resource Management with Residency Sets for more information.

## Topics

### Configuring the Residency Set

var label: String?

An optional name that can help you identify a residency set you create with the descriptor.

var initialCapacity: Int

The number of allocations a new residency set can store without reallocating memory.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Residency Sets

Simplifying GPU Resource Management with Residency Sets

Organize your resources into groups and influence when they become accessible to the GPU.

protocol MTLResidencySet

A collection of resource allocations that can move in and out of resident memory.

