

- Core Bluetooth
- CBCentralManager
-  connect(\_:options:) 

Instance Method

# connect(\_:options:)

Establishes a local connection to a peripheral.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func connect(
    _ peripheral: CBPeripheral,
    options: [String : Any]? = nil
)
```

## Parameters 

`peripheral`  

The peripheral to which the central is attempting to connect.

`options`  

A dictionary to customize the behavior of the connection. For available options, see Peripheral Connection Options.

## Discussion

After successfully establishing a local connection to a peripheral, the central manager object calls the centralManager(_:didConnect:) method of its delegate object. If the connection attempt fails, the central manager object calls the centralManager(_:didFailToConnect:error:) method of its delegate object instead. Attempts to connect to a peripheral don’t time out. To explicitly cancel a pending connection to a peripheral, call the cancelPeripheralConnection(_:) method. Deallocating `peripheral` also implicitly calls cancelPeripheralConnection(_:).

## See Also

### Establishing or Canceling Connections with Peripherals

Peripheral Connection Options

Keys used to pass options when connecting to a peripheral.

func cancelPeripheralConnection(CBPeripheral)

Cancels an active or pending local connection to a peripheral.

