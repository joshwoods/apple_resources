

- AudioDriverKit
- IOUserAudioCustomProperty
-  init 

Instance Method

# init

Initializes an instance of a custom property.

DriverKit 21.0+

``` source
bool init(IOUserAudioDriver * in_audio_driver, IOUserAudioObjectPropertyAddress in_prop_addr, bool in_is_property_settable, IOUserAudioCustomPropertyDataType in_qualifier_data_type, IOUserAudioCustomPropertyDataType in_data_type);
```

## Parameters 

`in_audio_driver`  

The IOUserAudioDriver that owns this object.

`in_prop_addr`  

The IOUserAudioObjectPropertyAddress of the custom property.

`in_is_property_settable`  

A Boolean value that indicates if the property can be set.

`in_qualifier_data_type`  

The IOUserAudioCustomPropertyDataType for custom property’s qualifier data value.

`in_data_type`  

The IOUserAudioCustomPropertyDataType for custom property’s data value.This value can’t be `IOUserAudioCustomPropertyDataType::None`.

## Return Value

`true` if initialization succeeded; `false` otherwise.

## See Also

### Creating a Custom Property

Create

Allocates and initializes an instance of the custom property class.

IOUserAudioObjectPropertyAddress

An object that collects the three parts — selector, scope, and element — that identify a specific property.

IOUserAudioCustomPropertyDataType

A data and qualifier type used for custom properties.

