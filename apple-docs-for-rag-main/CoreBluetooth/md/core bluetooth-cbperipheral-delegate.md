

- Core Bluetooth
- CBPeripheral
-  delegate 

Instance Property

# delegate

The delegate object specified to receive peripheral events.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any CBPeripheralDelegate)? { get set }
```

## Discussion

For information about how to implement your peripheral delegate, see CBPeripheralDelegate.

## See Also

### Identifying a Peripheral

var name: String?

The name of the peripheral.

