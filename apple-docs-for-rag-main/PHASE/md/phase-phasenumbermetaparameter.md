

- PHASE
-  PHASENumberMetaParameter 

Class

# PHASENumberMetaParameter

A metaparameter defined by a number that can change over time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASENumberMetaParameter
```

## Overview

This class contains a number that updates, like a “player speed” metaparameter that the app changes gradually from `0.0` to `1.0`.

To create an instance of this class, first create a PHASENumberMetaParameterDefinition, and either:

- Register it with the engine by calling registerGlobalMetaParameter(metaParameterDefinition:), then access the instance of this class in the engine’s globalMetaParameters dictionary.

- Pass it to the PHASEBlendNodeDefinition initializer, init(blendMetaParameterDefinition:identifier:), and then access the instance of this class in a sound event’s metaParameters dictionary.

- Use it as the input value for a PHASEMappedMetaParameterDefinition by passing it into the init(inputMetaParameterDefinition:envelope:) initializer. Then, access the instance of this class using the mapped parameter’s inputMetaParameterDefinition property.

## Topics

### Inspecting Extremes

var minimum: Double

The lowest possible number for the value.

var maximum: Double

The highest possible number for the value.

### Interpolating the Value

func fade(value: Double, duration: TimeInterval)

Sets the value gradually over the given amount of time.

## Relationships

### Inherits From

- PHASEMetaParameter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Linear Metaparameters

class PHASENumberMetaParameterDefinition

A specification for a metaparameter defined by a number.

