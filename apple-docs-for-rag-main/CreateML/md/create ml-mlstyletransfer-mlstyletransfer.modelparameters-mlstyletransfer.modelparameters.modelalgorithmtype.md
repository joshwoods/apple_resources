

- Create ML
- MLStyleTransfer
- MLStyleTransfer.ModelParameters
-  MLStyleTransfer.ModelParameters.ModelAlgorithmType 

Enumeration

# MLStyleTransfer.ModelParameters.ModelAlgorithmType

The style transfer training algorithm options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
enum ModelAlgorithmType
```

## Overview

This object uses a convolutional neural network for training the style transfer model, giving more detailed style It’s ideal for cases where latency is not the main concern, such as single images.

## Topics

### Selecting an algorithm type

case cnn

A style-transfer training algorithm that generates a model that prioritizes image quality over speed.

case cnnLite

A style-transfer training algorithm that generates a model that prioritizes speed over image quality.

### Describing an algorithm type

var description: String

A text representation of the model parameters.

var debugDescription: String

A text representation of the model parameters that’s suitable for output during debugging.

var playgroundDescription: Any

A description of the model parameters shown in a playground.

### Hashing an algorithm type

var hashValue: Int

func hash(into: inout Hasher)

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Working with raw values

init?(rawValue: String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Describing parameters

enum ValidationData

The source of a validation dataset for a style transfer model.

