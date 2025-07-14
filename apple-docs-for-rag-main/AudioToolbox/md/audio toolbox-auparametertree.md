

- Audio Toolbox
-  AUParameterTree 

Class

# AUParameterTree

An object that represents a top-level group node that contains all of an audio unit’s parameters.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AUParameterTree
```

## Overview

An audio unit’s parameters are organized into a tree containing groups and parameters (groups may be nested).

The parameter tree is KVO-compliant. An audio unit may choose to dynamically rearrange the tree; when doing so, it must issue a KVO notification on the audio unit’s parameterTree property.

## Topics

### Obtaining Tree Parameters

func parameter(withAddress: AUParameterAddress) -> AUParameter?

Searches the tree for a parameter with a specific address.

func parameter(withID: AudioUnitParameterID, scope: AudioUnitScope, element: AudioUnitElement) -> AUParameter?

Searches the tree for a specific version 2 audio unit parameter.

### Audio Unit Implementations

These methods are only of interest to audio unit subclasses.

class func createParameter(withIdentifier: String, name: String, address: AUParameterAddress, min: AUValue, max: AUValue, unit: AudioUnitParameterUnit, unitName: String?, flags: AudioUnitParameterOptions, valueStrings: [String]?, dependentParameters: [NSNumber]?) -> AUParameter

Creates a single parameter object.

class func createGroup(withIdentifier: String, name: String, children: [AUParameterNode]) -> AUParameterGroup

Creates a parameter group object.

class func createGroupTemplate([AUParameterNode]) -> AUParameterGroup

Creates a template group which may be used as a prototype for further group instances.

class func createGroup(fromTemplate: AUParameterGroup, identifier: String, name: String, addressOffset: AUParameterAddress) -> AUParameterGroup

Initializes a group as a copied instance of a template group.

class func createTree(withChildren: [AUParameterNode]) -> AUParameterTree

Creates a parameter tree object.

## Relationships

### Inherits From

- AUParameterGroup

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

class AUParameterGroup

A parameter group object represents a group of related audio unit parameters.

class AUParameterNode

An object that represents a node in an audio unit’s parameter tree.

