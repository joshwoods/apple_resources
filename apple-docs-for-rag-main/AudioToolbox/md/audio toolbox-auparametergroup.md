

- Audio Toolbox
-  AUParameterGroup 

Class

# AUParameterGroup

A parameter group object represents a group of related audio unit parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AUParameterGroup
```

## Overview

A parameter group is KVC-compliant for its children. For example, calling the parameter group’s value(forKey:) method, with a key value of *volume*, returns a child whose identifier value matches that key.

## Topics

### Obtaining Group Parameters

var allParameters: [AUParameter]

Returns a flat array of all parameters in the group, including those in child groups.

var children: [AUParameterNode]

The group’s child nodes.

## Relationships

### Inherits From

- AUParameterNode

### Inherited By

- AUParameterTree

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Parameters

class AUParameter

An object that represents a single audio unit parameter.

class AUParameterNode

An object that represents a node in an audio unit’s parameter tree.

class AUParameterTree

An object that represents a top-level group node that contains all of an audio unit’s parameters.

