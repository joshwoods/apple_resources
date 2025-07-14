

- PHASE
-  PHASEStringMetaParameter 

Class

# PHASEStringMetaParameter

A metaparameter with a text definition that can change over time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEStringMetaParameter
```

## Overview

This class contains text that updates, like a “weather” metaparameter that the app changes from “rainy” to “sunny.”

To create an instance of this class, first create a PHASEStringMetaParameterDefinition, and either:

- Register it with the engine by calling registerGlobalMetaParameter(metaParameterDefinition:), then access the instance of this class in the engine’s globalMetaParameters dictionary.

- Pass it to the PHASESwitchNodeDefinition initializer, init(switchMetaParameterDefinition:), and then access the instance of this class in a sound event’s metaParameters dictionary.

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

### Textual Metaparameters

class PHASEStringMetaParameterDefinition

A specification for a metaparameter defined by text.

