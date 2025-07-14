

- PHASE
-  PHASEStringMetaParameterDefinition 

Class

# PHASEStringMetaParameterDefinition

A specification for a metaparameter defined by text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEStringMetaParameterDefinition
```

## Overview

Use this class to spawn discrete instances of PHASENumberMetaParameter, for example, a “player speed” metaparameter that the app changes gradually from `0.0` to `1.0`.

To use a number metaparameter, create an instance of this class and:

- Register it with the engine by calling registerGlobalMetaParameter(metaParameterDefinition:), then access the instance of this class in the engine’s globalMetaParameters dictionary.

- Pass it to the PHASEBlendNodeDefinition initializer, init(blendMetaParameterDefinition:identifier:), and then access the instance of this class in a sound event’s metaParameters dictionary.

## Topics

### Creating a Parameter Definition

init(value: String)

Creates a specification for a textual metaparameter with the given value.

convenience init(value: String, identifier: String)

Creates a specification for a named textual metaparameter with the given value.

## Relationships

### Inherits From

- PHASEMetaParameterDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Textual Metaparameters

class PHASEStringMetaParameter

A metaparameter with a text definition that can change over time.

