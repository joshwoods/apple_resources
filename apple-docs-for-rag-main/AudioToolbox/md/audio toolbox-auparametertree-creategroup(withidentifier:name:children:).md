

- Audio Toolbox
- AUParameterTree
-  createGroup(withIdentifier:name:children:) 

Type Method

# createGroup(withIdentifier:name:children:)

Creates a parameter group object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class func createGroup(
    withIdentifier identifier: String,
    name: String,
    children: [AUParameterNode]
) -> AUParameterGroup
```

## Parameters 

`identifier`  

A non-localized, persistent identifier for the group.

`name`  

A localized display name for the group.

`children`  

The group’s child nodes.

## Return Value

A newly-initialized parameter group object.

## See Also

### Related Documentation

class AUParameterGroup

A parameter group object represents a group of related audio unit parameters.

### Audio Unit Implementations

class func createParameter(withIdentifier: String, name: String, address: AUParameterAddress, min: AUValue, max: AUValue, unit: AudioUnitParameterUnit, unitName: String?, flags: AudioUnitParameterOptions, valueStrings: [String]?, dependentParameters: [NSNumber]?) -> AUParameter

Creates a single parameter object.

class func createGroupTemplate([AUParameterNode]) -> AUParameterGroup

Creates a template group which may be used as a prototype for further group instances.

class func createGroup(fromTemplate: AUParameterGroup, identifier: String, name: String, addressOffset: AUParameterAddress) -> AUParameterGroup

Initializes a group as a copied instance of a template group.

class func createTree(withChildren: [AUParameterNode]) -> AUParameterTree

Creates a parameter tree object.

