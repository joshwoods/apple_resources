

- Accelerate
-  BNNSImageStackDescriptor Deprecated

Structure

# BNNSImageStackDescriptor

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
struct BNNSImageStackDescriptor
```

Deprecated

BNNS switched to new Layer Parameters data structures

## Overview

An image stack is a sequence of images with the same width and height. Each image in the sequence is called a channel. For example, a RGB image will be stored as three separate channels. A pixel has only one scalar value, stored using the type described by data_type.

Pixel P(c,x,y) at position (x,y) in channel c is stored in data\[x + row_stride \* y + image_stride \* c\], with x=0..width-1, y=0..height-1, c=0..channels-1. row_stride ≥ width, image_stride ≥ row_stride \* height.

Int types are converted to floating point using float Y = DATA_SCALE \* (float)X + DATA_BIAS, and back to integer using Int X = convert_and_saturate(Y / DATA_SCALE - DATA_BIAS)

## Topics

### Initializers

init()

init(width: Int, height: Int, channels: Int, row_stride: Int, image_stride: Int, data_type: BNNSDataType)

init(width: Int, height: Int, channels: Int, row_stride: Int, image_stride: Int, data_type: BNNSDataType, data_scale: Float, data_bias: Float)

### Instance Properties

var channels: Int

var data_bias: Float

var data_scale: Float

var data_type: BNNSDataType

var height: Int

var image_stride: Int

var row_stride: Int

var width: Int

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

struct BNNSVectorDescriptorDeprecated

