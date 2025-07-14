

- Audio Toolbox
- AUParameterTree
-  createParameter(withIdentifier:name:address:min:max:unit:unitName:flags:valueStrings:dependentParameters:) 

Type Method

# createParameter(withIdentifier:name:address:min:max:unit:unitName:flags:valueStrings:dependentParameters:)

Creates a single parameter object.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class func createParameter(
    withIdentifier identifier: String,
    name: String,
    address: AUParameterAddress,
    min: AUValue,
    max: AUValue,
    unit: AudioUnitParameterUnit,
    unitName: String?,
    flags: AudioUnitParameterOptions = [],
    valueStrings: [String]?,
    dependentParameters: [NSNumber]?
) -> AUParameter
```

## Parameters 

`identifier`  

The parameter’s non-localized, permanent name.

`name`  

The parameter’s localized name for display.

`address`  

The parameter’s address.

`min`  

The parameter’s minimum value.

`max`  

The parameter’s maximum value.

`unit`  

The parameter’s unit of measurement.

`unitName`  

The parameter’s localized unit name.

`flags`  

The parameter’s characteristic details.

`valueStrings`  

The parameter’s localized value strings.

`dependentParameters`  

Any other parameter’s whose values may change as a side effect of this parameter’s value changing.

## Return Value

A newly-initialized parameter object.

## See Also

### Related Documentation

class AUParameter

An object that represents a single audio unit parameter.

### Audio Unit Implementations

class func createGroup(withIdentifier: String, name: String, children: [AUParameterNode]) -> AUParameterGroup

Creates a parameter group object.

class func createGroupTemplate([AUParameterNode]) -> AUParameterGroup

Creates a template group which may be used as a prototype for further group instances.

class func createGroup(fromTemplate: AUParameterGroup, identifier: String, name: String, addressOffset: AUParameterAddress) -> AUParameterGroup

Initializes a group as a copied instance of a template group.

class func createTree(withChildren: [AUParameterNode]) -> AUParameterTree

Creates a parameter tree object.

