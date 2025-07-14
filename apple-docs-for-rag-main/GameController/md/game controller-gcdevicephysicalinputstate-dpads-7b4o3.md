

- Game Controller
- GCDevicePhysicalInputState
-  dpads 

Instance Property

# dpads

The device’s directional pads as key-value pairs for lookup by name.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS

``` source
var dpads: GCPhysicalInputElementCollection { get }
```

## See Also

### Accessing elements

var elements: GCPhysicalInputElementCollection&lt;any GCPhysicalInputElement>

The device’s elements as key-value pairs for lookup by name.

var axes: GCPhysicalInputElementCollection&lt;any GCAxisElement>

The device’s axes as key-value pairs for lookup by name.

var buttons: GCPhysicalInputElementCollection&lt;any GCButtonElement>

The device’s buttons as key-value pairs for lookup by name.

var switches: GCPhysicalInputElementCollection&lt;any GCSwitchElement>

The device’s switches as key-value pairs for lookup by name.

subscript(String) -> (any GCPhysicalInputElement)?

Returns the element that the key specifies.

**Required**

