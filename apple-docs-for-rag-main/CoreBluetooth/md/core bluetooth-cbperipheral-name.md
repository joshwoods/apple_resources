

- Core Bluetooth
- CBPeripheral
-  name 

Instance Property

# name

The name of the peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var name: String? { get }
```

## Discussion

Use this property to retrieve a human-readable name of the peripheral. A peripheral may have two different name types: one that the device advertises and another that the device publishes in its database as its Bluetooth low energy Generic Access Profile (GAP) device name. If a peripheral has both types of names, this property returns its GAP device name.

## Topics

### Related Documentation

func peripheralDidUpdateName(CBPeripheral)

Tells the delegate that a peripheral’s name changed.

## See Also

### Identifying a Peripheral

var delegate: (any CBPeripheralDelegate)?

The delegate object specified to receive peripheral events.

