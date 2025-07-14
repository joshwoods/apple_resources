

- Audio Toolbox
- AUParameterTree
-  createGroup(fromTemplate:identifier:name:addressOffset:) 

Type Method

# createGroup(fromTemplate:identifier:name:addressOffset:)

Initializes a group as a copied instance of a template group.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class func createGroup(
    fromTemplate templateGroup: AUParameterGroup,
    identifier: String,
    name: String,
    addressOffset: AUParameterAddress
) -> AUParameterGroup
```

## Parameters 

`templateGroup`  

A group to be used as a template and largely copied from.

`identifier`  

A non-localized, persistent identifier for the new group.

`name`  

A localized display name for the new group.

`addressOffset`  

The address offset for the new group’s parameters, with respect to the template group.

## Return Value

A newly-initialized parameter group object.

## See Also

### Audio Unit Implementations

class func createParameter(withIdentifier: String, name: String, address: AUParameterAddress, min: AUValue, max: AUValue, unit: AudioUnitParameterUnit, unitName: String?, flags: AudioUnitParameterOptions, valueStrings: [String]?, dependentParameters: [NSNumber]?) -> AUParameter

Creates a single parameter object.

class func createGroup(withIdentifier: String, name: String, children: [AUParameterNode]) -> AUParameterGroup

Creates a parameter group object.

class func createGroupTemplate([AUParameterNode]) -> AUParameterGroup

Creates a template group which may be used as a prototype for further group instances.

class func createTree(withChildren: [AUParameterNode]) -> AUParameterTree

Creates a parameter tree object.

