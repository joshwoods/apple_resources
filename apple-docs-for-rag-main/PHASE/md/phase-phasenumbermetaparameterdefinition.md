

- PHASE
-  PHASENumberMetaParameterDefinition 

Class

# PHASENumberMetaParameterDefinition

A specification for a metaparameter defined by a number.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASENumberMetaParameterDefinition
```

## Overview

Use this class to spawn discrete instances of PHASENumberMetaParameter, for example, a “player speed” metaparameter that the app changes gradually from `0.0` to `1.0`.

To use a number metaparameter, create an instance of this class and:

- Register it with the engine by calling registerGlobalMetaParameter(metaParameterDefinition:), then access the instance of this class in the engine’s globalMetaParameters dictionary.

- Pass it to the PHASEBlendNodeDefinition initializer, init(blendMetaParameterDefinition:identifier:), and then access the instance of this class in a sound event’s metaParameters dictionary.

- Pass it into the PHASEMappedMetaParameterDefinition initializer, init(inputMetaParameterDefinition:envelope:). Then, access the instance of this class using the mapped parameter’s inputMetaParameterDefinition property.

## Topics

### Creating a Metaparameter Definition

convenience init(value: Double)

Creates a specification for a metaparameter with the given numeric value.

convenience init(value: Double, identifier: String)

Creates a specification for a named metaparameter with the given numeric value.

init(value: Double, minimum: Double, maximum: Double)

Creates a specification for a metaparameter with the given numeric value and range.

convenience init(value: Double, minimum: Double, maximum: Double, identifier: String)

Creates a specification for a named metaparameter with the given numeric value and range.

### Reistricting the Value

var minimum: Double

The lowest possible number for the value.

var maximum: Double

The highest possible number for the value.

## Relationships

### Inherits From

- PHASEMetaParameterDefinition

### Inherited By

- PHASEMappedMetaParameterDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Linear Metaparameters

class PHASENumberMetaParameter

A metaparameter defined by a number that can change over time.

