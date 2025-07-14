

- PHASE
-  PHASEMetaParameterDefinition 

Class

# PHASEMetaParameterDefinition

A specification for a named parameter with a constant value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMetaParameterDefinition
```

## Overview

Instances of this class provide an app with dynamic control of various properies of live audio playback. This is a base class for the PHASENumberMetaParameterDefinition and PHASEStringMetaParameterDefinition subclasses.

You create a single instance of one of the subclasses for a specific property you want to adjust. By passing the definition subclass to the framework, you spawn one or more PHASEMetaParameterDefinition objects for discrete use across your app. For example, when you initialize a PHASEBlendNodeDefinition with a number metaparameter definition, PHASE registers a PHASENumberMetaParameter in the corresponding sound event’s metaParameters dictionary.

Put metaparameter definitions that you wish to share across different sounds in the asset registery’s globalMetaParameters dictionary. To add global metaparameter definitions to the dictionary, call registerGlobalMetaParameter(metaParameterDefinition:). Then pass the definition into several sound event node defintions, such as PHASESamplerNodeDefinition.

## Topics

### Setting a Metaparameter

var value: Any

A constant value for the parameter definition.

## Relationships

### Inherits From

- PHASEDefinition

### Inherited By

- PHASENumberMetaParameterDefinition
- PHASEStringMetaParameterDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Base Metaparameters

class PHASEMetaParameter

A named parameter with a value that the app can change over time.

class PHASEGlobalMetaParameterAsset

A reference to a registered metaparameter that the app can share with multiple sound events or sources.

