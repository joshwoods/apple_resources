

- Accelerate
-  BNNSSparsityParameters 

Structure

# BNNSSparsityParameters

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct BNNSSparsityParameters
```

## Overview

For BNNSSparsityTypeUnstructured, sparsity_ratio is numerator / denominator

## Topics

### Initializers

init()

init(flags: UInt64, sparsity_ratio: (UInt32, UInt32), sparsity_type: BNNSSparsityType, target_system: BNNSTargetSystem)

### Instance Properties

var flags: UInt64

var sparsity_ratio: (UInt32, UInt32)

var sparsity_type: BNNSSparsityType

var target_system: BNNSTargetSystem

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct BNNSDataType

BNNS Data Types.

struct BNNSSparsityType

struct BNNSTargetSystem

struct bnns_graph_argument_t

Describes data associated with an input or output argument

struct BNNSImageStackDescriptorDeprecated

struct BNNSVectorDescriptorDeprecated

