

- AudioDriverKit
- IOUserAudioCustomProperty
-  Create 

Static Method

# Create

Allocates and initializes an instance of the custom property class.

DriverKit 21.0+

``` source
static OSSharedPtr Create(IOUserAudioDriver * in_audio_driver, IOUserAudioObjectPropertyAddress in_prop_addr, bool in_is_property_settable, IOUserAudioCustomPropertyDataType in_qualifier_data_type, IOUserAudioCustomPropertyDataType in_data_type);
```

## Parameters 

`in_audio_driver`  

The IOUserAudioDriver that owns this object.

`in_prop_addr`  

IOUserAudioObjectPropertyAddress of the custom property.

`in_is_property_settable`  

A Boolean value that indicates if the property can be set.

`in_qualifier_data_type`  

The IOUserAudioCustomPropertyDataType for custom property’s qualifier data value.

`in_data_type`  

The IOUserAudioCustomPropertyDataType for custom property’s data value.This value can’t be `IOUserAudioCustomPropertyDataType::None`.

## Return Value

A poiner to an IOUserAudioCustomProperty, if allocation and initialization succeeded.

## Discussion

If you subclass IOUserAudioCustomProperty to override this class’ behavior, don’t use Create to allocate and initialize the custom subclass.

## See Also

### Creating a Custom Property

init

Initializes an instance of a custom property.

IOUserAudioObjectPropertyAddress

An object that collects the three parts — selector, scope, and element — that identify a specific property.

IOUserAudioCustomPropertyDataType

A data and qualifier type used for custom properties.

