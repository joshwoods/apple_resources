

- Audio Toolbox
- AUParameterTree
-  createGroupTemplate(\_:) 

Type Method

# createGroupTemplate(\_:)

Creates a template group which may be used as a prototype for further group instances.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class func createGroupTemplate(_ children: [AUParameterNode]) -> AUParameterGroup
```

## Parameters 

`children`  

The template group’s child nodes.

## Return Value

A newly-initialized parameter group template.

## Discussion

Template groups provide a way to construct multiple instances of identical parameter groups, sharing certain immutable state between the instances.

Template groups may not appear in trees except at the root.

## See Also

### Audio Unit Implementations

class func createParameter(withIdentifier: String, name: String, address: AUParameterAddress, min: AUValue, max: AUValue, unit: AudioUnitParameterUnit, unitName: String?, flags: AudioUnitParameterOptions, valueStrings: [String]?, dependentParameters: [NSNumber]?) -> AUParameter

Creates a single parameter object.

class func createGroup(withIdentifier: String, name: String, children: [AUParameterNode]) -> AUParameterGroup

Creates a parameter group object.

class func createGroup(fromTemplate: AUParameterGroup, identifier: String, name: String, addressOffset: AUParameterAddress) -> AUParameterGroup

Initializes a group as a copied instance of a template group.

class func createTree(withChildren: [AUParameterNode]) -> AUParameterTree

Creates a parameter tree object.

