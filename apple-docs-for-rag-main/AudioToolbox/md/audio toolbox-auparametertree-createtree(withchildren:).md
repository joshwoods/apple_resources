

- Audio Toolbox
- AUParameterTree
-  createTree(withChildren:) 

Type Method

# createTree(withChildren:)

Creates a parameter tree object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class func createTree(withChildren children: [AUParameterNode]) -> AUParameterTree
```

## Parameters 

`children`  

The tree’s top-level children nodes.

## Return Value

A newly-initialized parameter tree object.

## See Also

### Related Documentation

class AUParameterTree

An object that represents a top-level group node that contains all of an audio unit’s parameters.

### Audio Unit Implementations

class func createParameter(withIdentifier: String, name: String, address: AUParameterAddress, min: AUValue, max: AUValue, unit: AudioUnitParameterUnit, unitName: String?, flags: AudioUnitParameterOptions, valueStrings: [String]?, dependentParameters: [NSNumber]?) -> AUParameter

Creates a single parameter object.

class func createGroup(withIdentifier: String, name: String, children: [AUParameterNode]) -> AUParameterGroup

Creates a parameter group object.

class func createGroupTemplate([AUParameterNode]) -> AUParameterGroup

Creates a template group which may be used as a prototype for further group instances.

class func createGroup(fromTemplate: AUParameterGroup, identifier: String, name: String, addressOffset: AUParameterAddress) -> AUParameterGroup

Initializes a group as a copied instance of a template group.

