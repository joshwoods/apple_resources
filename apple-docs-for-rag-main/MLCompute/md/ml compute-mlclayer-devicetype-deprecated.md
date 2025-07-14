

- ML Compute
- MLCLayer
-  deviceType Deprecated

Instance Property

# deviceType

A device type that indicates where the system executes the layer.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
var deviceType: MLCDeviceType { get }
```

## Discussion

The system uses the MLCDevice you provide to compile(options:device:) to execute the layers in the graph.

If you select MLCDeviceType.ane, it is possible that some layers may not execute on the MLCDeviceType.ane, but instead on the CPU or GPU.

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

class func supportsDataType(MLCDataType, on: MLCDevice) -> Bool

Returns a Boolean that indicates whether instances of this layer accept source tensors for the data type and device that you specify.

Deprecated

