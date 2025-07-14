

- PHASE
-  PHASEMetaParameter 

Class

# PHASEMetaParameter

A named parameter with a value that the app can change over time.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
class PHASEMetaParameter
```

## Overview

Instances of this class provide an app with dynamic control of a sound’s properties. A metaparameter takes a single value as input and may operate on one or more audio characteristics.

To change the value of a metaparameter at runtime:

- Assign a string to a textual metaparameter’s value.

- Adjust the value of a number or mapped metaparameter gradually over a duration by calling fade(value:duration:).

## Topics

### Accessing the Value

var value: Any

A value for the metaparameter.

### Identifying the Parameter

var identifier: String

A unique name for the metaparameter.

## Relationships

### Inherits From

- NSObject

### Inherited By

- PHASENumberMetaParameter
- PHASEStringMetaParameter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Base Metaparameters

class PHASEMetaParameterDefinition

A specification for a named parameter with a constant value.

class PHASEGlobalMetaParameterAsset

A reference to a registered metaparameter that the app can share with multiple sound events or sources.

