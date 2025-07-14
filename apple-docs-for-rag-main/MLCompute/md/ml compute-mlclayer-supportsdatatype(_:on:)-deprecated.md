

- ML Compute
- MLCLayer
-  supportsDataType(\_:on:) Deprecated

Type Method

# supportsDataType(\_:on:)

Returns a Boolean that indicates whether instances of this layer accept source tensors for the data type and device that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class func supportsDataType(
    _ dataType: MLCDataType,
    on device: MLCDevice
) -> Bool
```

## Parameters 

`dataType`  

The data type of a possible input tensor to the layer.

`device`  

The device to use to determine layer support.

## Return Value

`true` if the specified data type and device are supported.

## See Also

### Inspecting a Layer

var layerID: Int

A unique number that identifies each layer.

Deprecated

var label: String

A string that helps identify this layer.

Deprecated

var isDebuggingEnabled: Bool

A Boolean that indicates whether you choose to debug the layer when executing a graph that includes it.

Deprecated

var deviceType: MLCDeviceType

A device type that indicates where the system executes the layer.

Deprecated

