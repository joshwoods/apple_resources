

- Core Bluetooth
- CBPeripheralDelegate
-  peripheralDidUpdateName(\_:) 

Instance Method

# peripheralDidUpdateName(\_:)

Tells the delegate that a peripheral’s name changed.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralDidUpdateName(_ peripheral: CBPeripheral)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

## Discussion

Core Bluetooth invokes this method whenever the peripheral’s Generic Access Profile (GAP) device name changes. Since a peripheral device can change its GAP device name, you can implement this method if your app needs to display the current name of the peripheral device.

## See Also

### Monitoring Changes to a Peripheral’s Name or Services

func peripheral(CBPeripheral, didModifyServices: [CBService])

Tells the delegate that a peripheral’s services changed.

