

- Enterprise Program API
-  Device 

Object

# Device

The data structure that represents a Devices resource.

``` source
object Device
```

## Properties

`attributes`

Device.Attributes

The resource’s attributes.

`id`

`string`

 (Required) 

The opaque resource ID that uniquely identifies the resource.

`type`

`string`

 (Required) 

The resource type.

Value: `devices`

`links`

ResourceLinks

Navigational links that include the self-link.

## Attributes 

Possible types:

## Topics

### Objects

object Device.Attributes

Attributes that describe a Devices resource.

## See Also

### Objects

object DevicesWithoutIncludesResponse

object DeviceCreateRequest

The request body you use to create a Device.

object DeviceUpdateRequest

The request body you use to update a Device.

object DeviceResponse

A response that contains a single Devices resource.

object DevicesResponse

A response that contains a list of Devices resources.

