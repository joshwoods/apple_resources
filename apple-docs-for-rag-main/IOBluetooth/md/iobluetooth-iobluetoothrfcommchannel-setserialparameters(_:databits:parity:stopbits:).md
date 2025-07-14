

- IOBluetooth
- IOBluetoothRFCOMMChannel
-  setSerialParameters(\_:dataBits:parity:stopBits:) 

Instance Method

# setSerialParameters(\_:dataBits:parity:stopBits:)

Changes the parameters of the serial connection.

macOS

``` source
func setSerialParameters(
    _ speed: UInt32,
    dataBits nBits: UInt8,
    parity: BluetoothRFCOMMParityType,
    stopBits bitStop: UInt8
) -> IOReturn
```

## Parameters 

`speed`  

The baudrate.

`nBits`  

Number of data bits.

`parity`  

The type of parity can be NoParity, OddParity, EvenParity or MaxParity.

`bitStop`  

Number of stop bits.

## Return Value

An error code value. 0 if successful.

