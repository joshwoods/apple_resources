

- Core Bluetooth
- CBCentralManager
-  cancelPeripheralConnection(\_:) 

Instance Method

# cancelPeripheralConnection(\_:)

Cancels an active or pending local connection to a peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cancelPeripheralConnection(_ peripheral: CBPeripheral)
```

## Parameters 

`peripheral`  

The peripheral to which the central manager is either trying to connect or has already connected.

## Discussion

This method is nonblocking, and any CBPeripheral class commands that are still pending to `peripheral` may not complete. Because other apps may still have a connection to the peripheral, canceling a local connection doesn’t guarantee that the underlying physical link is immediately disconnected. From the app’s perspective, however, the peripheral is effectively disconnected, and the central manager object calls the centralManager(_:didDisconnectPeripheral:error:) method of its delegate object.

## See Also

### Establishing or Canceling Connections with Peripherals

func connect(CBPeripheral, options: [String : Any]?)

Establishes a local connection to a peripheral.

Peripheral Connection Options

Keys used to pass options when connecting to a peripheral.

