

- ML Compute
- MLCLayer
-  isDebuggingEnabled Deprecated

Instance Property

# isDebuggingEnabled

A Boolean that indicates whether you choose to debug the layer when executing a graph that includes it.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var isDebuggingEnabled: Bool { get set }
```

## Discussion

If `true`, the layer makes the result tensor and gradient tensors available for reading. The default value is `false`.

Important

If you set `isDebuggingEnabled` to `true`, make sure to also include debugLayers in the `options` parameter when compiling the graph. Otherwise the layer ignores this property.

## See Also

### Inspecting a Layer

var layerID: Int

A unique number that identifies each layer.

Deprecated

var label: String

A string that helps identify this layer.

Deprecated

var deviceType: MLCDeviceType

A device type that indicates where the system executes the layer.

Deprecated

class func supportsDataType(MLCDataType, on: MLCDevice) -> Bool

Returns a Boolean that indicates whether instances of this layer accept source tensors for the data type and device that you specify.

Deprecated

