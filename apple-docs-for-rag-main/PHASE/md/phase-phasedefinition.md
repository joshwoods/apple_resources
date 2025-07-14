

- PHASE
-  PHASEDefinition 

Class

# PHASEDefinition

A base class that adds a name to framework definitions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEDefinition
```

## Overview

Various PHASE classes derive from this class, for example, PHASEMixerDefinition, PHASEMetaParameterDefinition, and PHASESoundEventNodeDefinition.

This class represents a template from which PHASE creates concrete PHASEAsset subclasses at runtime. For example, when you register a global metaparameter definition using registerGlobalMetaParameter(metaParameterDefinition:), PHASE returns a PHASEAsset subclass, PHASEGlobalMetaParameterAsset, that identifies a usable metaparameter by name. To access the usable metaparameter, pass the PHASEGlobalMetaParameterAsset identifier into the globalMetaParameters dictionary.

## Topics

### Identifying a Definition

var identifier: String

A unique name for the definition.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PHASEMetaParameterDefinition
- PHASEMixerDefinition
- PHASESoundEventNodeDefinition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Audio Layering and Effects

class PHASEChannelMixerDefinition

An audio-layering object that routes sound directly to the device’s output.

class PHASEAmbientMixerDefinition

An audio-layering object that outputs sound in a particular direction in 3D space.

class PHASEMixerDefinition

An object to initialize a mixer with a given configuration.

class PHASEMixer

An object that combines multiple audio signals into a single signal.

Spatial Mixing

Define environmental characteristics that determine how sound plays in your app’s 3D soundscape.

