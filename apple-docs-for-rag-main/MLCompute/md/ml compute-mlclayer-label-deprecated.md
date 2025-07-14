

- ML Compute
- MLCLayer
-  label Deprecated

Instance Property

# label

A string that helps identify this layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var label: String { get set }
```

## See Also

### Inspecting a Layer

var layerID: Int

A unique number that identifies each layer.

Deprecated

var isDebuggingEnabled: Bool

A Boolean that indicates whether you choose to debug the layer when executing a graph that includes it.

Deprecated

var deviceType: MLCDeviceType

A device type that indicates where the system executes the layer.

Deprecated

class func supportsDataType(MLCDataType, on: MLCDevice) -> Bool

Returns a Boolean that indicates whether instances of this layer accept source tensors for the data type and device that you specify.

Deprecated

