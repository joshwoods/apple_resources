

- PHASE
-  PHASEGlobalMetaParameterAsset 

Class

# PHASEGlobalMetaParameterAsset

A reference to a registered metaparameter that the app can share with multiple sound events or sources.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEGlobalMetaParameterAsset
```

## Overview

The engine’s registerGlobalMetaParameter(metaParameterDefinition:) function returns an instance of this class for a parameter you register. Then, you access the actual metaparameter by using this class’s identifier as the key for metaparameter dictionary, for example, a sound event’s metaParameters or the asset registry’s globalMetaParameters.

As an opaque derived object, this class adds no properties to the subclass.

## Relationships

### Inherits From

- PHASEAsset

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

class PHASEMetaParameterDefinition

A specification for a named parameter with a constant value.

