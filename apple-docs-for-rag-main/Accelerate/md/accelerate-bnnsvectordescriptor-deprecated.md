

- Accelerate
-  BNNSVectorDescriptor Deprecated

Structure

# BNNSVectorDescriptor

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
struct BNNSVectorDescriptor
```

Deprecated

BNNS switched to new Layer Parameters data structures

## Overview

Represents a vector of dimension size. Each vector element is a scalar value, stored using the type specified in data_type.

Component V(i) at index i is stored in data\[i\], with i=0..size-1.

Int types are converted to floating point using float Y = DATA_SCALE \* (float)X + DATA_BIAS, and back to integer using Int X = convert_and_saturate(Y / DATA_SCALE - DATA_BIAS)

## Topics

### Initializers

init()

init(size: Int, data_type: BNNSDataType)

init(size: Int, data_type: BNNSDataType, data_scale: Float, data_bias: Float)

### Instance Properties

var data_bias: Float

var data_scale: Float

var data_type: BNNSDataType

var size: Int

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Structures

struct BNNSDataType

BNNS Data Types.

struct BNNSSparsityParameters

struct BNNSSparsityType

struct BNNSTargetSystem

struct bnns_graph_argument_t

Describes data associated with an input or output argument

struct BNNSImageStackDescriptorDeprecated

