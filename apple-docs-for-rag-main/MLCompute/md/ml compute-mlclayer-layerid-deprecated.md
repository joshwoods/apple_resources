

- ML Compute
- MLCLayer
-  layerID Deprecated

Instance Property

# layerID

A unique number that identifies each layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var layerID: Int { get }
```

## Discussion

The framework assigns `layerID` during layer initialization.

## See Also

### Inspecting a Layer

var label: String

A string that helps identify this layer.

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

