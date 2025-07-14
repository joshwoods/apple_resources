

- Game Controller
- GCDevicePhysicalInputState
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the element that the key specifies.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
subscript(key: String) -> (any GCPhysicalInputElement)? { get }
```

**Required**

## Parameters 

`key`  

A key that identifies an element.

## Return Value

The element that matches the key.

## See Also

### Accessing elements

var elements: GCPhysicalInputElementCollection&lt;any GCPhysicalInputElement>

The device’s elements as key-value pairs for lookup by name.

var axes: GCPhysicalInputElementCollection&lt;any GCAxisElement>

The device’s axes as key-value pairs for lookup by name.

var buttons: GCPhysicalInputElementCollection&lt;any GCButtonElement>

The device’s buttons as key-value pairs for lookup by name.

var dpads: GCPhysicalInputElementCollection&lt;any GCDirectionPadElement>

The device’s directional pads as key-value pairs for lookup by name.

var switches: GCPhysicalInputElementCollection&lt;any GCSwitchElement>

The device’s switches as key-value pairs for lookup by name.

